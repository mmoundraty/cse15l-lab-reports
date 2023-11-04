## Part 1

~~~
@Test 
	public void testReverseInPlace() {
    int[] input1 = {5, 6, 7,8};
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{8, 7, 6, 5}, input1);
	}
~~~

~~~
public void testReverseInPlace() {
    int[] input1 = {5, 6, 7,8};
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{8, 7, 7, 8}, input1);
	}
~~~

~~~
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }
~~~
