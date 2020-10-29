# Linear Search

    Short Intro: Element to be searched is compared with every element till a match is found.

    Best Case Time complexity: O(1);
    Worst Case Time complexity: O(N), where N is the number of element in the array.
    Space Complexity: O(1)

    For more Info: https://www.geeksforgeeks.org/binary-search/
 
# Jump Search
    Short Intro: It is performed on sorted data, array is divided into M parts and we find in which part our element would lie and then we do linear search to find the desired element.

    Best Case Time Complexity: O(1).
    Worst Case Time Complexity: O(sqrt(N)), where N is the lenth of the array. Algorithm works optimal when we take M = sqrt(N).
    Space Complexity: O(1)

    Advantage: Works better than linear search for sorted array.

    For more info: https://www.geeksforgeeks.org/jump-search/

# Binary Search

    Short Intro: Based on Divide and Conquer Technique. Works on sorted array, we compare the searched value with middle value of the array and find out in which part of the array it can be present right half or left half, similarly we do it recursively till we found the element or we have exhausted the array. 

    Best Case Time Complexity: O(1).
    Worst Case Time Complexity: O(log(N)), where N is the lenth of the array.
    Space Complexity: O(1)

    For more info: https://www.geeksforgeeks.org/binary-search/

# Exponential Search

    Short Intro:  It is used in place where upper bound of array size is very large. We find the part where searched element would lie and then perform binary search onthe part to find the element. The part size grow exponentiallly in order of 2, like 0-2, 2-4, 4-8, 8-16....

    Best Case Time Complexity: O(1).
    Worst Case Time Complexity: O(log(N)), where N is the lenth of the array.
    Space Complexity: O(1)

    For more info: https://www.geeksforgeeks.org/exponential-search/?ref=lbp
