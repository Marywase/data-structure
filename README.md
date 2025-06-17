# Algorithm

## Problem 1: Sum of Distinct Elements

### Description

Given two sets (arrays), find the sum of all distinct elements — i.e., elements present in either of the sets but not in both.

### Algorithm

```text
Algorithm: Sum_Of_Distinct_Elements(A, B)
Input: Two arrays A and B
Output: Sum of elements that are in either A or B, but not both

1. Initialize sum ← 0
2. For i from 0 to length of A - 1 do
      If A[i] is not in B then
          sum ← sum + A[i]
3. For j from 0 to length of B - 1 do
      If B[j] is not in A then
          sum ← sum + B[j]
4. Return sum


Procedure: Dot_Product(v1, v2, ps)
Input: Arrays v1 and v2 of same length, ps passed by reference
Output: ps contains the dot product

1. Set ps ← 0
2. For i from 0 to length of v1 - 1 do
      ps ← ps + (v1[i] × v2[i])
3. End


Algorithm: Check_Orthogonality_Procedure(V1, V2, n)

1. For i from 0 to n - 1 do
      Call Dot_Product(V1[i], V2[i], ps)
      If ps = 0 then
          Print "Vectors i are orthogonal"
      Else
          Print "Vectors i are NOT orthogonal"
2. End


Function: Dot_Product(v1, v2)

1. Set ps ← 0
2. For i from 0 to length of v1 - 1 do
      ps ← ps + (v1[i] × v2[i])
3. Return ps

Algorithm: Check_Orthogonality_Function(V1, V2, n)

1. For i from 0 to n - 1 do
      result ← Dot_Product(V1[i], V2[i])
      If result = 0 then
          Print "Vectors i are orthogonal"
      Else
          Print "Vectors i are NOT orthogonal"
2. End
```
