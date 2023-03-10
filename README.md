# Recursion
Write a C++ program to which will create a static array of size 10 now pass this array to a function 
which will print the array elements using recursion.

 #include<iostream>
 using namespace std;
 void print_arr(int ar[],int s)
 {
 	if(s==0)
 	{
 		cout<<ar[0]<<endl;
 		return;
	}
	else 
	{	
	cout<<ar[s]<<endl;
	print_arr(ar,s-1);
    } 
	
 }
 int main()
 {
 	int a[10];
 	cout<<"Enter the elements in an array "<<endl;
 	for(int i=0;i<10;i++)
 	{
 		cin>>a[i];
	}
	print_arr(a,10);
 }
