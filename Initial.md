
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

## Functions
