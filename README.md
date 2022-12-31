# Palindromic-Numbers-C++

# Problem 1: Palindromic Numbers
A palindromic number is one that reads the same both ways, from the beginning or from the end. For example, 525 and 8448 are palindromic numbers. Note that 525 and 8448 are also products of two 2-digit numbers: 525 = 15 * 35 and 8448 = 96 * 88. On the other hand, 7777 is a palindromic number but not a product of two 2-digit numbers.
Write a C++ program that prompts the user for two integers M and N and output numbers in the range of M and N (inclusively) which are either (1) palindromic only; (2) product of two 3-digit numbers only; or (3) both palindromic and product of two 3-digit numbers.
```
Input:
• A single line containing two integers M , N , and a char opt for the display option.
• You may assume that M <= N and both numbers are within the range 10000 to 999999 (inclusively), and opt must be one of the chars 'p' , 't' , 'b' .
Output:
• If the input opt is the char 'p' , then output the palindromic numbers in the range of M and N (inclusively) in increasing order.
• If the output opt is the char 't' , then output the numbers which are a product of two 3-digit numbers in the range of M and N (inclusively) in increasing order.
• If the input opt is the char 'b' , then output the numbers which are both palindromic and a product of two 3-digit numbers in the range of M and N (inclusively) in increasing order.
• If there is no number within the range that matches the criteria, no line will be output.
Requirement:
• Your program must implement the following two helper functions:
◦ bool isPalindrome(int x) which returns whether the parameter x
is a palindromic number.
◦ bool isProduct(int x) which returns whether the parameter x is
a product of two 3-digit numbers.
• Call the helper functions in your main function to accomplish the task.
• You can ONLY use the simple data types char , bool , int , double . In other
words, you are not allowed to use other data types or data structures such as arrays, strings or STL containers (e.g., vectors), etc.
Sample Test Cases

```

```
User inputs are shown in blue. 1_1
10000 10300 p
  10001
  10101
  10201
       
1_2
 10000 10300 t
  10000
  10100
  10200
  10201
  10300
1_3
10000 10300 b
10201
1_4
  99000 110000 b
  99099
  99199
  99299
  99599
  99699
  99799
  99899
  99999
  101101
  102201
  105501
  106601
  108801
1_5 (Note: there is no output in this test case) 100000 101000 b

```
   
