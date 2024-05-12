# DSA
#include <stdio.h>
void bubbleSort(int arr[], int n){
    for(int i = 0;i < n; i++){
        for(int j = 0 ; j < n - i -1; j++){
            if( arr[j] > arr[j+1])
            {
                int temp=arr[j];
                arr[j]=arr[j+1];
                arr[j+1]=temp;
            }
        }
    }
}

int main() 
{
	int a[] = {40,60,20,10,30,70,60,50};
	bubbleSort(a, 8);
	for(int i = 0;i < 8; i++){
	    printf("%d ",a[i]);
	}
	return 0;
}
// code for bubble sort
