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
## PROBLEM:02

```c
#include <stdio.h>
#include <stdlib.h>
#define MAX_HEIGHT 41

struct box
{
	int length;
    int width;
    int height;
};

typedef struct box box;

int get_volume(box b) {
	return b.length*b.width*b.height;
}

int is_lower_than_max_height(box b) {
    if(b.height<MAX_HEIGHT){
        return 1;
    }
    else{
        return 0;
    }
}

int main()
{
	int n;
	scanf("%d", &n);
	box *boxes = malloc(n * sizeof(box));
	for (int i = 0; i < n; i++) {
		scanf("%d%d%d", &boxes[i].length, &boxes[i].width, &boxes[i].height);
	}
	for (int i = 0; i < n; i++) {
		if (is_lower_than_max_height(boxes[i])) {
			printf("%d\n", get_volume(boxes[i]));
		}
	}
	return 0;
}

```
