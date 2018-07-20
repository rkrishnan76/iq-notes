# iq-notes

1. Dailiy Coding Problem#1.Given a list of numbers and a number k, return whether any two numbers from the list add up to k.

Ans: Sort the array. Start from leftmost element and add it the last element.
      if the sum is equal you found the match.  
      if the sum is less increment the leftmost element index
      if the sum is more decrement the rightmost element index.

2. Given a node find the right side if exists: courtesy:https://www.geeksforgeeks.org/find-next-right-node-of-a-given-key/
      need to maintain two queues. 1 for adding and removing the nodes and 2. for maintaining the level

3. Given the root to a binary tree, implement serialize(root), which serializes the tree into a string, and deserialize(s), which deserializes the string back into the tree.

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


