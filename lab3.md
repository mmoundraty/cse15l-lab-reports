## Part 1

~~~
@Test 
public void testReverseInPlace() {
    int[] input1 = {5, 6, 7, 8};
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{8, 7, 6, 5}, input1);
	}
~~~

~~~
public void testReverseInPlace() {
    int[] input1 = {5, 6, 7, 8};
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{8, 7, 7, 8}, input1);
	}
~~~

![Image](15ljava1.png)

~~~
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }
~~~

~~~
static void reverseInPlace(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[i];
    }
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
  }
~~~

The fix in the new code block addresses the issue that the array does not copy its changed elements. By creating a new array you can pick the elements that are unchanged in `newArray` into the original array in reversed order without overlapping.

