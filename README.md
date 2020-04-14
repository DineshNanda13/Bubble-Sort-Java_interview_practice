# Bubble-Sort-Java_interview_practice
In bubble sort algorithm, array is traversed from first element to last element. Here, current element is compared with the next element. If current element is greater than the next element, it is swapped.
package com.bubbleSort;

/**
 *
 * @author Dinesh Nanda
 */

public class BubbleSort {

    public static void main(String[] args) {
        
        int arr[] ={3,60,35,2,45,320,5};  
        
        for(int i = 0; i < arr.length; i++){
            for(int j = 1; j < arr.length; j++){
                
                if(arr[j-1] > arr[j]){
                    int temp = arr[j-1];
                    arr[j-1] = arr[j];
                    arr[j] = temp;
                }
            }
        }
        for(int i = 0; i < arr.length; i++){
            System.out.print(arr[i]+" ");
        }
        
    }
    
}
