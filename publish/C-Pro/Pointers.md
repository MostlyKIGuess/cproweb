
- They store the [[Memory Address]] of a variable.
- Usually if it's a 32 bit pointer it has the size of 4 bytes.
- It is somewhat of a data type. It's format specifier is "%p".
- If we use "%d" specifier it would print the hexadecimal address to an integer address.
```c
#include <stdio.h>

int main(){
    int a=5;
	    printf("%p\n",&a); outputs : 00000000005ffe9c
	    print("%d\n",&a);  outputs : 6291100
    return 0;
}
```









