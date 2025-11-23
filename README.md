# HackerRank.problems (STRUCT)

## PROBLEM:01

```c
#include <stdio.h>

struct student{
    char first_name[51] = {'j','o', 'h', 'n'};
    char last_name[51] = {'c','a','r','m','a','c','k'};
    int age = 15;
    int standard = 10;
}student;

int main() {
    
    printf("%d %s %s %d", student.age, student.first_name, student.last_name, student.standard);
    
    return 0;
}
```
