# Lab Report 1
# Part 2

## The bug from reverseInPlace method in ArrayExamples.java

Original codes for reverseInPlace method:
```
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {   
      arr[i] = arr[arr.length - i - 1];
    }
}
```

## 1. A failure-inducing input for the buggy program

The JUnit test:
```
@Test
public void testReverseInPlace2() {
    int[] input2 = {2,3,4,5,0};
    ArrayExamples.reverseInPlace(input2);
    assertArrayEquals(new int[]{0,5,4,3,2}, input2);
}
```
The input is {2,3,4,5,0}

The expected output is {0,5,4,3,2} 

The actual output is {0,5,4,5,0}

## 2. An input that doesn’t induce a failure

The JUnit test:
```
@Test
public void testReverseInPlace() { 
    int[] input1 = {0};    
    ArrayExamples.reverseInPlace(input1);    
    assertArrayEquals(new int[]{0}, input1);    
}
  ```
The input is {0}

The expected output is {0} 

The actual output is {0}

## 3. The symptom, as the output of running the tests 
 
 Using the two inputs above:
 ![Image](Screen Shot 2023-01-29 at 16.09.17.png)
 
 The output of running the test:
 ![Image](Screen Shot 2023-01-29 at 16.09.42.png)
 
## 4. The bug, as the before-and-after code change required to fix it

The before-code:
```
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {   
      arr[i] = arr[arr.length - i - 1];
    }
}
```

The after-code that fix the bug:
```
static void reverseInPlace(int[] arr) {
    int[] newArray = new int[arr.length];
    for (int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[i];
    }
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
}
 ```
The reason why the reverseInPlace method is buggy is mainly becuase when it iterates through every element in the arr by reversing order, 
the element in arr in each index is also changed accordingly. So the elements we get from arr during for loop is no longer in their original 
order or position. Thus, to fix the problem, we first need to make a newArray that contains all the elements in arr with the same length. By 
this way, we can deeply copy the input - arr and make sure all the elements that we extract later will be in their original order. Then to 
change the order of elements, we can employ for loop to iterate through all the elements that saved in newArray in reversing order and 
replace them sequentially in arr.

# Part 3
One thing I learned from Lab 2 was that we can literaly write a web server using java in Visual Studio Code. More interestingly, we can write
specific codes to make web server support the path and behavior based on what we want to display. What's more, except running web server on
our local machine, we can also run it remotely, this says we can also access the web server using remote computers, which is very cool to learn.

