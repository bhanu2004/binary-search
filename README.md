//binary-search
#include <iostream>


using namespace std;

int main()
{
int n;
cin>>n;
int arr[n];
for(int i=0;i<n;i++)cin>>arr[i];
int fir=0,las=n-1,mid,check;
cout<<"finding number: ";
cin>>check;
while(fir<=las){
    mid=(fir+las)/2;
    if(arr[mid]==check){
        cout<<"position: "<<mid+1;
        break;
    }
    if(arr[mid]<check){
        fir=mid;
    }
    if(arr[mid]>check){
        las=mid;
    }
}

return 0;

}
