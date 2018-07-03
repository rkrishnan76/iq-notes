# iq-notes

1. Dailiy Coding Problem#1.Given a list of numbers and a number k, return whether any two numbers from the list add up to k.

Ans: Sort the array. Start from leftmost element and add it the last element.
      if the sum is equal you found the match.  
      if the sum is less increment the leftmost element index
      if the sum is more decrement the rightmost element index.

2. Given the root to a binary tree, implement serialize(root), which serializes the tree into a string, and deserialize(s), which deserializes the string back into the tree.
