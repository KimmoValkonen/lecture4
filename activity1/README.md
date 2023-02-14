# Activities

## Task 1

- Refer to the following link. Discuss how Merge-sort works:
  https://opendsa-server.cs.vt.edu/OpenDSA/AV/Sorting/mergesortAV.html
- Merge-sort Practice. Refer to the following link. Merge the two sub-arrays into the larger array.
  https://opendsa-server.cs.vt.edu/OpenDSA/Exercises/Sorting/MergesortMergePRO.html
  # A: Merge Sort is a divide-and-conquer algorithm that sorts an array of elements by recursively dividing the array into two halves, sorting each half, and then merging the two sorted halves back into a single sorted array.

## Task 2

- Refer to the following link. Discuss how Quick-sort works:  
  https://opendsa-server.cs.vt.edu/OpenDSA/AV/Sorting/quicksortAV.html
- Quick-sort Practice. Refer to the following link. Partition the array using quicksort.
  https://opendsa-server.cs.vt.edu/OpenDSA/Exercises/Sorting/QuicksortPartitPRO.html
  # A: QuickSort is a divide-and-conquer algorithm that sorts an array of elements by selecting a pivot element, partitioning the array around the pivot element, and recursively sorting the two partitioned arrays.

## Task 3

- The following snippet is from `./src/quicksort.cpp` lines 32-43. Discuss in groups how the code works:

```cpp
void quickSort(int arr[], int low, int high)
{
    if (low < high)
    {
        //partition the array
        int pivot = partition(arr, low, high);

        //sort the sub arrays independently
        quickSort(arr, low, pivot - 1);
        quickSort(arr, pivot + 1, high);
    }
}
```
# A: Recursively sorting the two partitioned arrays around the pivot element

- The following snippet is from `./src/quicksort.cpp` line 27. Discuss in groups how ìt works:

```cpp
swap(&arr[i + 1], &arr[high]);
```
# A: It swaps the values stored at the memory locations pointed to by the pointers &arr[i + 1] and &arr[high].

## Task 4: Individual (at home)

1. Merge-sort has better worst case performance than quicksort. So why Quick-sort is considered better than Merge-sort? Refer to the following article
   https://www.geeksforgeeks.org/quicksort-better-mergesort/
   # A: Quicksort worst case can be brought down to Mergesort with selecting pivot by taking average from 3 elements O(n2). Quick-sort requires little space. No additional storage space is needed to perform sorting. Merge sort requires a temporary array to merge the sorted arrays.
2. Refer to the following article. Analyze the complexity of the Merge-sort algorithm.
   https://www.softwaretestinghelp.com/merge-sort/
   # A: The total time to perform merge sort will be n(log n+1), which gives us the time complexity of O(nlogn). Merge-sort

    Worst case time complexity	O(n*log n)
    Best case time complexity	O(n*log n)
    Average time complexity	O(n*log n)
    Space complexity	O(n)

3. Refer to the following article. Analyze the complexity of the Quick-sort algorithm.
   https://www.softwaretestinghelp.com/quick-sort/
   # A: Worst case: O(n2), Best case: O(nlogn), Average case: also becomes O(nlogn)
   Quick-sort

    Worst case time complexity	O(n 2 )
    Best case time complexity	O(n*log n)
    Average time complexity	O(n*log n)
    Space complexity	O(n*log n)
