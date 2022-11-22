#include<iostream>
using namespace std;
void deletion(int arr[],int n,int k){
int temp;
for(int i=0; i<n; i++){
    if(arr[i]==k){
        temp = i;
        break;
    }
}


for(int i=temp; i<n; i++){
    arr[i]=arr[i+1];
}
}
int main(){
  std::cout<<"array:";
    int arr[]={2,3,4,2,4,2};
    int n =6;
for(int i=0; i<n; i++){
    std::cout<<arr[i]<<" ";
}    
cout<<endl;
cout<<"enter the element want to delete:";
int k ; cin>>k;
deletion(arr,n,k);
std::cout<<"new array:";
for(int i=0; i<n-1; i++){
    cout<<arr[i]<<" ";
}
return 0;
}
