1.

The disaggregate function is splitting an array into multiple parts based on a given depth value, which gives the number of levels into which the array should be split.
In each function call, the array is split into two arrays: the smaller array and the bigger array. The smaller array contains values that are smaller than the average of the values in the full array and the bigger array contains values that are bigger than the average of the values in the full array.
Since the function is recursive, it  takes the smaller array and repeats the same process of splitting it into another smaller array and another bigger array (this also happens for the bigger array).

2.

The space used in the stack will increase with larger arrays and larger depth values. Larger arrays require more values to be stored on the stack, which is why they'll use more stack space. Larger depth values require more function calls, which means that more space will be needed in the 'buffer' portion of the stack.