# iq-notes

1. Dailiy Coding Problem#1.Given a list of numbers and a number k, return whether any two numbers from the list add up to k.

Ans: Sort the array. Start from leftmost element and add it the last element.
      if the sum is equal you found the match.  
      if the sum is less increment the leftmost element index
      if the sum is more decrement the rightmost element index.

2. Given a node find the right side if exists: courtesy:https://www.geeksforgeeks.org/find-next-right-node-of-a-given-key/
      need to maintain two queues. 1 for adding and removing the nodes and 2. for maintaining the level

3. Given the root to a binary tree, implement serialize(root), which serializes the tree into a string, and deserialize(s), which deserializes the string back into the tree. ()
https://www.programcreek.com/2014/05/leetcode-serialize-and-deserialize-binary-tree-java/
the above link has:
LeetCode – Binary Search Tree Iterator (Java)
LeetCode – Binary Tree Right Side View (Java)
LeetCode – Balanced Binary Tree (Java)
LeetCode – Invert Binary Tree (Java)

4. reservoir sampling - https://en.wikipedia.org/wiki/Reservoir_sampling
ReservoirSample(S[1..n], R[1..k])
  // fill the reservoir array
  for i = 1 to k
      R[i] := S[i]

  // replace elements with gradually decreasing probability
  for i = k+1 to n
    j := random(1, i)   // important: inclusive range--generate a number between 1 & for eg., 11 if it is less than equal 10 replace that element with the 11th element.
    if j <= k
        R[j] := S[i]

5. Given an array of integers, return a new array such that each element at index i of the new array is the product of all the numbers in the original array except the one at i.
Solution: https://www.geeksforgeeks.org/a-product-array-puzzle/
    while iterating forward,  prod[i] = temp;temp *= arr[i]; while backward, prod[i] *= temp; temp *= arr[i];
    
6. Find missing positive integer.
      1. remove the negative no.s and construct new array.
      2. In the constructed array, make the no. negative for the location @ arr[i] if it is greater than zero
      if(Math.abs(arr[i]) - 1 < size && arr[Math.abs(arr[i]) - 1] > 0)
          arr[Math.abs(arr[i]) - 1] = -arr[Math.abs(arr[i]) - 1];



7. Running Mean.
      Construct new array and order them as you read from the provided array.  This can be done by comparing with the prior no.s and moving them to the right position.

8. finding all subset of a given set.

