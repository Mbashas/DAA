# DDA
All my work related to design and analysis of algorithm.  

#QUICK SORT 
Quick sort is a highly efficient, comparison-based sorting algorithm that follows the divide-and-conquer strategy. It works by selecting a pivot element from the array and partitioning the other elements into two sub-arrays, according to whether they are less than or greater than the pivot. The sub-arrays are then recursively sorted, and the process continues until the entire array is sorted. Quick sort is a popular sorting algorithm that follows the divide-and-conquer approach. It works by selecting a pivot element from the array and partitioning the other elements into two sub-arrays based on whether they are less than or greater than the pivot. The sub-arrays are then recursively sorted. Quicksort algorithm works:
Pivot Selection: Choose a pivot element from the array. There are various ways to choose a pivot, such as selecting the first, last, or middle element. The choice of pivot can affect the efficiency of the algorithm, but for simplicity, let's assume we select the last element as the pivot.
Partitioning: Rearrange the array such that all elements less than the pivot are placed before it, and all elements greater than the pivot are placed after it. This step is also known as partitioning. To do this, maintain two pointers, i and j, initially pointing to the first element of the array.
Iterate j from the first element to the second-to-last element of the array.
Recursive Sort: Recursively apply the above two steps to the sub-arrays on both sides of the pivot (i.e., the elements to the left and right of the pivot) until the sub-arrays contain only one element or are empty.
Apply the Quicksort algorithm to the sub-array from index 0 to i-1 (left of the pivot).
Apply the Quicksort algorithm to the sub-array from index i+1 to the last element (right of the pivot).
Combine: The sub-arrays are now sorted. The elements on the left of the pivot are all less than the pivot, and the elements on the right are all greater than the pivot. As a result, the entire array is sorted.
Termination: The recursion terminates when the sub-arrays have zero or one element, as they are already sorted by definition.

#Counting Sort
Counting sort is a sorting algorithm that sorts the elements of an array by counting the number of occurrences of each unique element in the array. The count is stored in an auxiliary array and the sorting is done by mapping the count as an index of the auxiliary array. Counting Sort Algorithm works by:
Find out the maximum element (let it be max) from the given array.
Initialize an array of length max+1 with all elements 0. This array is used for storing the count of the elements in the array.
Store the count of each element at their respective index in count arrayFor example: if the count of element 3 is 2 then, 2 is stored in the 3rd position of count array. If element “5” is not present in the array, then 0 is stored in 5th position.
Store cumulative sum of the elements of the count array. It helps in placing the elements into the correct index of the sorted array.
Find the index of each element of the original array in the count array. This gives the cumulative count. Place the element at the index calculated as shown in 
After placing each element at its correct position, decrease its count by one.

#Heap Sort
Heapsort is a comparison-based sorting algorithm. where we first find the minimum element and place the minimum element at the beginning. Repeat the same process for the remaining elements. The heap sort algorithm has limited uses because Quicksort and Merge sort are better in practice.
Heap data structures have a number of applications due to their ability to provide fast access to the smallest or largest element in a collection.
Heap sort is one of the sorting algorithms used to arrange a list of elements in order. The Heapsort algorithm uses one of the tree concepts called Heap Tree. In this sorting algorithm, we use Max Heap to arrange the list of elements in Descending order and the Min Heap to arrange the list of elements in Ascending order.
We need to perform three concepts these are Mean Heap, Max Heap, and Heapify Let’s know what is,
Mean Heap: In a Min-Heap the key present at the root node must be less than or equal among the keys present at all of its children. In a Min-Heap the minimum key element is present at the root.
Max Heap: In a Max-Heap the key present at the root node must be greater than or equal among the keys present at all of its children. In a Max-Heap the maximum key element is present at the root.
Heapify: It is the process of creating a heap data structure from a binary tree. It is used to create a Min-Heap or a Max-Heap.
The Heap sort algorithm to arrange a list of elements in ascending order is performed these steps:
Construct a Binary Tree with the given list of Elements.
Transform the Binary Tree into Max Heap.
Delete the root element from Max Heap using the Heapify method.
Put the deleted element into the Sorted list.
Repeat the same until Max Heap becomes empty.
Display the sorted list.
