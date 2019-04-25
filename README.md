# BubbleSort
Day 20 - Sorting an Array of Integers using Bubble Sort

The array is already sorted, so  swaps take place and we print the necessary  lines of output shown above.

Sample Input 1

3  
3 2 1  

Sample Output 1

Array is sorted in 3 swaps.  
First Element: 1  
Last Element: 3  

Based on this code example:

for (int i = 0; i < n; i++) {
    // Track number of elements swapped during a single array traversal
    int numberOfSwaps = 0;
    
    for (int j = 0; j < n - 1; j++) {
        // Swap adjacent elements if they are in decreasing order
        if (a[j] > a[j + 1]) {
            swap(a[j], a[j + 1]);
            numberOfSwaps++;
        }
    }
    
    // If no elements were swapped during a traversal, array is sorted
    if (numberOfSwaps == 0) {
        break;
    }
}
