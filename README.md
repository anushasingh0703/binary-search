# binary-search
# Binary-Search

A sorted array can be searched using the binary search algorithm by continually halving the search interval. Utilising the knowledge that the array is sorted, binary search attempts to minimise the time complexity to O(log N).

Conditions for when to apply Binary Search in a Data Structure:
To apply binary search in any data structure, the data structure must maintain the following properties:

The data structure must be sorted.

Access to any element of the data structure takes constant time.

How to Implement Binary Search?
The basic steps to perform Binary Search are:
a) Set the low index to the first element of the array and the high index to the last element.

b) Set the middle index to the average of the low and high indices.

c) If the element at the middle index is the target element, return the middle index.

d) Otherwise, based on the value of the key to be found and the value of the middle element, decide the next search space.

e) If the target is less than the element at the middle index, set the high index to middle index – 1.

f) If the target is greater than the element at the middle index, set the low index to middle index + 1.

g) Perform step 2 repeatedly until the target element is found or the search space is exhausted.

![234096323-95b91936-60ce-4899-b4f8-48166f6fd618](https://user-images.githubusercontent.com/125882453/234392773-e500257e-d3eb-4c0a-9d26-980b4a44192c.png)

The Binary Search Algorithm can be implemented in the following two ways
Iterative Binary Search Algorithm

Recursive Binary Search Algorithm

Example of Pseudocode of Iterative Binary Search Algorithm:
binarySearch(arr, x, low, high)
    repeat till low = high
           mid = (low + high)/2
           if (x = arr[mid])
               return mid
          else if (x > arr[mid])
               low = mid + 1
          else
               high = mid – 1
               
 Advantages of Binary Search:
Binary search is faster than linear search, especially for large arrays. As the size of the array increases, the time it takes to perform a linear search increases linearly, while the time it takes to perform a binary search increases logarithmically.

Binary search is more efficient than other searching algorithms that have a similar time complexity, such as interpolation search or exponential search.

Binary search is relatively simple to implement and easy to understand, making it a good choice for many applications.

Drawbacks of Binary Search:
1.We require the array to be sorted. If the array is not sorted, we must first sort it before performing the search. This adds an additional O(N * logN) time complexity for the sorting step, which makes it irrelevant to use binary search.

2.Binary search requires that the data structure being searched be stored in contiguous memory locations. This can be a problem if the data structure is too large to fit in memory, or if it is stored on external memory such as a hard drive or in the cloud.

3.Binary search requires that the elements of the array be comparable, meaning that they must be able to be ordered. This can be a problem if the elements of the array are not naturally ordered, or if the ordering is not well-defined.

Applications of Binary Search:
1.Binary search can be used as a building block for more complex algorithms used in machine learning, such as algorithms for training neural networks or finding the optimal hyperparameters for a model.

2.Commonly used in Competitive Programming.

3.Can be used for searching in computer graphics. Binary search can be used as a building block for more complex algorithms used in computer graphics, such as algorithms for ray tracing or texture mapping.

4.Can be used for searching a database. Binary search can be used to efficiently search a database of records, such as a customer database or a product catalog.
