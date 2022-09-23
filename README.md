# ***🌟Give Star If you find this helpful :)🌟***

# 1. ***Code Binary Search***
### Code:Code Binary Search
public class Solution { 

    public static int binarySearch(int[] arr, int x) {
        int temp = -1,start=0,end=arr.length-1;
        
        while (start <= end) {
            int mid = (start + end) / 2;
            if (arr[mid] < x) {
                start = mid + 1;
            } else if (arr[mid] == x) {
                temp = mid;
                break;
            } else {
                end = mid - 1;
            }
            
        }
        if (start > end)
          {  temp = -1;}
        return temp;
    }
    
}

# 2. ***Selection sort***
### Code:Selection sort
public class Solution {  

    public static void selectionSort(int[] arr) {
    	 for (int i = 0; i < arr.length - 1; i++) {
            for(int j=i+1;j<arr.length;j++){
                if (arr[i] > arr[j]) {
                    int min = arr[j];
                    arr[j] = arr[i];
                    arr[i] = min;
                }
            }     
        }
    }   

}

# 3. ***Code Bubble Sort***
### Code:Code Bubble Sort
public class Solution {  

    public static void bubbleSort(int[] arr){
    	     for (int i = 0; i < arr.length; i++) {
            for (int j = 1; j < arr.length-i; j++) {
                if (arr[j-1] > arr[j]) {
                    int temp = arr[j-1];
                    arr[j-1] = arr[j];
                    arr[j] = temp;
                }
            }
        }
    }  

}

# 4. ***Code Merge Two Sorted Arrays***
### Code:Code Merge Two Sorted Arrays
public class Solution {  

    public static int[] merge(int arr1[], int arr2[]) {
        int arr3[]=new int[arr1.length+arr2.length];
        int i=0;
        int j=0;
        int k=0;
        while(i<arr1.length && j<arr2.length){
          if(arr1[i]<arr2[j])
          {
              arr3[k]=arr1[i];
              k++;
              i++;
          }
            else{
              arr3[k]=arr2[j];
              k++;
              j++;
            }
        }
        while(i<arr1.length)
        {
            arr3[k]=arr1[i];
            k++;
            i++;        
        
        }
        while(j<arr2.length)
        {
         arr3[k]=arr2[j];
            k++;
            j++;    
        }
        return arr3;
    }

}


# ***🌟Give Star If you find this helpful :)🌟***
