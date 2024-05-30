# ArrayInsertAtPos
Insert an element in an array at a specific position given by user
//Insert an element in array at given position
#include<iostream>
using namespace std;

int main(){
	int n ;
	cout<<"Enter the size of array: ";
	cin>>n;
	int arr[n];
	for(int i=0;i<n;i++){
		cin>>arr[i];
	}
	int pos;
	cout<<"Enter position: ";
	cin>>pos;
	int x;
	cout<<"Enter element: ";
	cin>>x;
	n=n+1;
	for(int i=n-1;i>=pos;i--){
		arr[i]=arr[i-1];
	}
	arr[pos]=x;
	for(int i=0;i<n;i++){
		cout<<arr[i]<<" ";
	}
}
