





// Insertion sort
#include <stdio.h>

int main() {
    int i,j,n,key,arr[30];
    // Taking size of array
    printf("Enter the size of an Array:\n");
    scanf("%d",&n);
    
    //Taking array elements
    printf("Enter the array elements \n");
    for(i=0;i<n;i++)
    {
    scanf("%d",&arr[i]);
    }
    
    //printing array
    printf("The array elements are: \n");
    for(j=0;j<n;j++)
    {
        printf("%d \t",arr[j]);
    }
    
    printf("\n");
    //Alogorihtm
    for(j=1;j<n;j++)
    {
        key=arr[j];
        i=j-1;
        
        while(i>=0 && arr[i]>key)
        {
            arr[i+1]=arr[i];
            i=i-1;
        }
        arr[i+1]=key;
    }
    
    //print soreted array
    printf("The sorted array in asecending: \n");
    for(j=0;j<n;j++)
    {
        printf("%d \t",arr[j]);
    }
    printf("\n");
         printf("The sorted array in descending: \n");
    for(j=n-1;j>=0;j--)
    {
        printf("%d \t",arr[j]);
    }
   
    return 0;
}
