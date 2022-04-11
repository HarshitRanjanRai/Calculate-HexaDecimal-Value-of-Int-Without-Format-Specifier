#include<stdio.h>
#include<ctype.h>

int main()
{
	int a,arr[10],d,i=0;
	scanf("%d",&a);
	
	while(a>0)
	{
		d=a%16;
		arr[i]=d;
		 a=a/16;
		 i++;
	}
	for(;i>=0;i--)
	{
		d=arr[i];
		if(d>=0&&d<=9)
		printf("%d ",d);
		else
		{
			if(d==10)
			printf("A");
			if(d==11)
			printf("B");
			if(d==12)
			printf("C");
			if(d==13)
			printf("D");
			if(d==14)
			printf("E");
			if(d==15)
			printf("F");
			
		}
	}
	
	return 0;
}
