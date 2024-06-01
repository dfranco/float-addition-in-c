# Float variables addition in most languages (proof in C language)

This piece of C code demonstrates why when we add 0.1 and 0.2, we obtain a different result than expected.

## Code

```c
#include <stdio.h>

int main(void) {
  float y = 0.1;
  float x = 0.2;
  float z = x + y;

  printf("\nz = %.12f\n",z);
}
```

Above C code, we add 0.1 and 0.2 using float, and display the result using printf with 12 decimals precision.

## Code compilation

Compiling the code is simple as running

`gcc main.c -o main`

## Execution and output

Execute the program by running

`./main`

with output

```shell
z = 0.300000011921
```

The expected result would be 0.3, but a good explanation can be found using below link in reference.

Enjoy!

## References

[Why 0.1 + 0.2 Doesn’t Equal 0.3 in Most Programming Languages](https://builtin.com/articles/0-1-0-2#:~:text=JavaScript%20doesn't%20define%20different,to%20the%20equation%20becomes%200.30000000000000004%20.)
