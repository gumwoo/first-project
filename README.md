"# My project" 


#include<stdio.h>

int find_max4(int a, int b, int c, int d);

int main(){
	int x1, x2, x3, x4, max;
	
	scanf("%d %d %d %d", &x1, &x2, &x3, &x4);
	
	max= find_max4(x1,x2,x3,x4);
	printf("최대는 %d이다.\n", max);
	
	return 0;
} 

int find_max4(int a, int b, int c, int d){
	int maximum;
	
	if(a>b && a>c && a>d) maximum=a;
	else if (b>a && b>c && b>d) maximum=b;
	else if (c>a && c>b && c>d) maximum=a;
	else maximum=d;
	
	return maximum;
}
