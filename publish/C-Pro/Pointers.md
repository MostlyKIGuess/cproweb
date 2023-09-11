
- They store the [[Memory Address]] of a variable.
- Usually if it's a 32 bit pointer it has the size of 4 bytes.
- It is somewhat of a data type. It's format specifier is "%p".
- If we use "%d" specifier it would print the hexadecimal address to an integer address.
```c
#include <stdio.h>

int main(){
    int a=5;
	    printf("%p\n",&a); outputs : 00000000005ffe9c
	    printf("%d\n",&a);  outputs : 6291100
    return 0;
}
```

```c
int *a = &b;
and 
int *a;
a = &b;
while those both are same but 
int *a;
*a = &b;

is a different thing.
```

### Array Pointer
Name of [[Arrays]] is a **constant** pointer to the address of the first element of the array.
```c
arr = &arr[0]
```

You can not modify/change that pointer that is it uses
const type of stuff so you can't add 1 or perform operations on it.



It kind of points the whole array so when we print
```c
printf("%d\n"&a + 1)
```
This will give out the output of memory address of a + 4*(size of array)

assuming array is of int type that's why it is multiplied by 4.


![[pointers.excalidraw]]

```c
   Pointer to an integer`

    int *p;

    Pointer to an array of 5 integers

    int (*ptr)[5];

    int arr[5];

     Points to 0th element of the arr.

    p = arr;

    Points to the whole array arr.

    ptr = &arr;
```


[[Double Pointers]]
