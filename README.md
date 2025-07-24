# Leetcode-1662. Check If Two String Arrays are Equivalent

# Description

Given two string arrays word1 and word2, return true if the two arrays represent the same string, and false otherwise.

A string is represented by an array if the array elements concatenated in order forms the string.

# Solution

In this problem we are given 2 strings word1 and word2 . We need to check whether the concatanation of these 2 strings are equal . If they are equal then return True or else return False.

For example :

1 .word1 = ["ab", "c"], word2 = ["a", "bc"]

abc = abc 

Hence, True

2 .word1 = ["a", "cb"], word2 = ["ab", "c"]

acb not equals abc

Hence , False

# Algorithm

1. Use join() function to join the substrings into 1 string in word 1 .
2. Repeat the same procedure in word 2 as well.
3. Now check if they are equal or not , If they are same then return True else return False.

# Code 
class Solution:

    def arrayStringsAreEqual(self, word1: List[str], word2: List[str]) -> bool:
        w1=''.join(word1)
        w2=''.join(word2)
        return w1==w2
# time Complexity

''.join(word1) function takes O(n) where n is total number of characters in word1.

''.join(word1) function takes O(n) where n is total number of characters in word1.

Hence the total time complexity is :

O(n+m)
