
## Pointers
```C
#include <stdio.h>
int main()
{
    int i=10;
    p= &i;  //p hold the address of i
    *p= 20; // Modifies i through p 
    printf("i =%d", i); //i =20
    return 0;
}
```
`sizeof(p)` ------> 4 bytes or 8 bytes (depending if the system is 32 bit one or 64 bit one)  
`sizeof(*p)` -----> int/float/char.....

## Arrays
**Initalizing:**  

`float f[4]` An array declared that contains 4 floating point values.  
```
int a[5] = {22, 37, 3490};  // The rest are initialized to 0
```
Or,
```
int a[10] = {0, 11, 22, [5]=55, 66, 77};
```
If Out of Bounds ------> Undefined Behaviour  


**Size:** 
```C
int x[12];
printf("%zu\n", sizeof(x));  // Total bytes of the array
printf("%zu\n", sizeof(int)); // Size of each element
printf("%zu\n", sizeof(x) / sizeof(int));  // Number of elements in the array
```
But if you pass the array to a function, you only pass a pointer to the first element, so sizeof(x) will not work as expected.

**Multi-dimensional Array**
`int b[2][4] //2D Array with 2 rows and 4 columns`
