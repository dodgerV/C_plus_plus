#include <iostream>
#include <string.h>
 
using namespace std;

void fill(int* pa,int size_a)
{
	int i;
	for(i=0;i<size_a;i++)
	{
		*(pa+i)=i*2-i;
	}	
}

void fill(double* pb,int size_b)
{
	int i,j;
	for(i=0;i<size_b;i++)
	{
		for(j=0;j<size_b;j++)
		{
			*((double*)pb+size_b*i+j)=i*2+0.2*j;
		}	
	}
}

void show(int* pa,int size_a)
{

	int i;
	for(i=0;i<size_a;i++)
	{
		cout<<*(pa+i)<<" ";
	}
	cout<<'\n';
	cout<<'\n';
}

void show(double* pb,int size_b)
{

	int i,j;
	for(i=0;i<size_b;i++)
	{
		for(j=0;j<size_b;j++)
		{
			cout<<*((double*)pb+size_b*i+j)<<" ";
		}	
		cout<<'\n';
	}
	cout<<'\n';
}

void show(char* ps, int size_c)
{
	int i;
	for(i=0;i<size_c;i++)
	{
		cout<<*(ps+i);
	}
	cout<<'\n';
	cout<<'\n';

}

int* sort(int* pa,int size_a)
{
	int i,j,temp=0;
	
	for(i=0;i<size_a;i++)
	{

	 for(j=i+1; j<size_a;j++)
	 {
	 	if(*(pa+j)>*(pa+i))
	 	{
	 		temp=*(pa+j);
	 			*(pa+j)=*(pa+i);
	 			*(pa+i)=temp;
	 	}
	 }
	}
	return pa;
}

double* sort(double* pb,int size_b)
{
	int i,j,k;
	double temp=0;


for(k=0;k<size_b;k++)
{
	for(i=0;i<size_b;i++)
	{
	 
	 	for(j=i+1; j<size_b;j++)
	 	{
	 		if(*(pb+size_b*k+j)>*(pb+size_b*k+i))
	 		{
	 			temp=*(pb+size_b*k+j);
	 			*(pb+size_b*k+j)=*(pb+size_b*k+i);
	 			*(pb+size_b*k+i)=temp;
	 		}
	 	}
	}
}
	return pb;
}

char* sort(char* ps,int size_c)
{
	int i,j;
	char temp;
	
	for(i=0;i<size_c;i++)
	{

	 for(j=i+1; j<size_c;j++)
	 {
	 	if(*(ps+j)<*(ps+i))
	 	{
	 		temp=*(ps+j);
	 			*(ps+j)=*(ps+i);
	 			*(ps+i)=temp;
	 	}
	 }
	}	
	return ps;
}

int main()
{
	const int size_b=4;
	const int size_a=10;
	const int size_c=10;

	double b[4][4];
	int a[10];
	char s[10]="gpidpkwa";

	double* pb=NULL;
	int* pa=NULL;
	char* ps=NULL;

	pa=&a[0];
	pb=&b[0][0];
	ps=&s[0];

	fill(pa,size_a);
	show(pa,size_a);
	pa=sort(pa,size_a);
	show(pa,size_a);

	fill(pb,size_b);
	show(pb,size_b);
	pb=sort(pb,size_b);
	show(pb,size_b);

	show(ps,size_c);
	ps=sort(ps,size_c);
	show(ps,size_c);

	return 0;
}
