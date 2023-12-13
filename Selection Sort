#include<stdio.h>
int main(){
	int size=0,temp=0,i=0,j=0;
	printf("Please enter the size of the array: ");
	scanf("%d", &size);
	int arr[size];
	
	for(i=0;i<size;i++){
		printf("\nPlease enter the element no %d: ",i+1);
		scanf("%d",&arr[i]);
	}
	//To check the number of passes and comparisons
	int pass=0,comp=0,swap=0;
	
	//Implementation of selection sort
	for(i=0;i<size-1;i++){
		int minIdx = i;
		for(j=i+1;j<size;j++) {if(arr[minIdx]>arr[j]) minIdx = j;comp++;}
		if(minIdx!=i){
			temp = arr[i];
			arr[i] = arr[minIdx];
			arr[minIdx] = temp;
			swap++;
		}
		pass++;
	}
	printf("\nThe number of passes = %d and the number of swaps = %d and no. of comparisons = %d",pass,swap,comp);
	printf("\nThe array after sorting is: ");
	for(i=0;i<size;i++) printf("%d ", arr[i]);
	return 0;
}
