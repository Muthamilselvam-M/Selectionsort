# Selectionsort

import java.util.Arrays;
public class Main
{
	public static void main(String[] args) {
		int[] arr = {2,4,56,21,1};
		insertion(arr);
		System.out.println(Arrays.toString(arr));
	}
	public static void insertion(int[] arr){
	    for(int i=0;i<arr.length-1;i++){
	        for(int j=i+1;j>0;j--){
	            if(arr[j] < arr[j-1]){
	                swap(arr,j,j-1);
	            }
	            else{
	                break;
	            }
	        }
	    }
	}
	public static void swap(int[] arr,int s1,int s2){
	    int temp = arr[s1];
	    arr[s1] = arr[s2];
	    arr[s2] = temp;
	}
}
