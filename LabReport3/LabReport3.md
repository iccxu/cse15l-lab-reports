Part 1 - Bugs
Choose one of the bugs from week 4’s lab.

Provide:

- A failure-inducing input for the buggy program, as a JUnit test and any associated code (write it as a code block in Markdown)
- An input that doesn’t induce a failure, as a JUnit test and any associated code (write it as a code block in Markdown)
- The symptom, as the output of running the tests (provide it as a screenshot of running JUnit with at least the two inputs above)
- The bug, as the before-and-after code change required to fix it (as two code blocks in Markdown)
- Briefly describe why the fix addresses the issue.

**Part 1 - Bugs**
When testing with JUnit, the program would not properly reverse the elements of the list in both the `reversed` and `reversedInPlace` methods. For this example, I'll refer to the `reversedInPlace` method. A failure-inducing input for the buggy program from week 4's lab was as simple as a regular list such as `{1, 2, 3}`. The code for the `reversedInPlace` method prior to fixing and my test follows:  
```
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }

@Test 
public void testReverseInPlace3Items() {
    int[] input1 = {1, 2, 3};
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{3, 2, 1}, input1);
}
```
This test resulted in an incorrectly ordered list error where the last element was '3' when it should've been '1'.  

```
  @Test 
	public void testReverseInPlaceSameNums() {
    int[] input1 = {1, 1, 1};
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{1, 1, 1}, input1);
	}
```
However, the input of a list with the same element value passes the test such as `{1, 1, 1}`. This is because the list element values remain the same regardless of if it was actually reversed or not. Below is the JUnit results of both the failing and passing test:  
![Image](lab3_JUnit_test.png)

