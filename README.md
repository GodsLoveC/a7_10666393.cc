
//CPP program to find element
//closet to a given target
#include <iostream>

using namespace std;

int getClosest(int,int,int);
int findClosest(int arr,int n,int target)
{

   if(target<= arr[0])
        return arr[0];
    if (target>= arr[n-1])
       return arr[n-1];
    //Doing binary search
    int i+0, j+n, mid=0
    while(i<j){
        mid(i+j)/2;
        if(arr[mid]==target)
  return arr[mid];
  /*if target is less than array element search in left*/
          if(arr[mid]<target)
            {
            //i target is greater than the previous
             //to mid return closest to two
             if(mid>0&&target>arr[mid-1])
             return getClosest(arr[mid-1],arr[mid],target);
             /*repeat for the left half*/
             j=mid;
          }//if target is greater than mid
             else{
                 if(mid<n-1&&target<arr[mid+1])
                 return getClosest(,arr[mid],arr[mid+1],target);
             i= mid +1
             }
    }//only single element left after search
    return arr[mid];

    int getClosest(int val1,int val2,int target
    {
        if (target - val1>=val2-target)
        return val2;
        else
        return val2;

}
 //driver code
 int main()
 {
     int arr[={1,2,4,5,6,6,8,9};
     int n= sizeof(arr)/sizeof(arr[0]);
     int target=11;
     cout<<(findClosest(arr,n,target));
 }

}
