# W2
算法

(1). A sorted array supports fast search (using binary search) but slow insertion when we must retain sorted order.

     True. Binary search, in contrast, makes O(log2n) comparisons in the worst case.
   
(2). Given an unsorted singly-linked list L of n items, which one of the following statements is False. Note that a singly-linked list is a linked list in which each node contains a single pointer to the next node in sequence.
     
     False. Insertion and deletion of an item I are both O(1) operations (worst case). While insertion of an item into an unsorted singly-linked list is an O(1) operation in the worst case, deletion of an item is not. Deletion has a worst case complexity of O(n).
     
(3). Ignore

(4). This function uses a curious mix of iteration and recursion:

         function F(n)
          if n < 1
             return 1
          t <- 0
          for i <- 0 to n
                 for j <- i to n
                        t <- t + j
          return t + F(n-1)
         two for loop running till n which will give us complexity of n^2 , the last main recursive function again 
         which will again run till n, So in total it gives us the complexity of n^3 .
         
         fn=f1+f2+...fn-1+nt，每个f的base cases数量为当前n的平方，1²加2²加。。。n²，n(n+1)(2n+1)/6
         
        
(5). Given two functions f(n)=n^2 and g(n)=n , which of the following statement is correct?
     
     f(n) has a higher growth rate than g(n)
     
(6). In Lecture 5 we discussed the brute-force approach to string search. 
How many character comparisons will the algorithm make when searching for 'lido' in the string 'supercalifragilisticexpialidocious' ?
     
     33. 7+3(lif)+6+3(lis)+10+4(lido)=33
     
(7). One of my books has 589 pages, numbered consecutively. Every page has a page number, the first being 1. 
How many decimal digits were used to type the 589 page numbers? 

    The first 9 pages are number with 1-9 = 9 decimals and then starts with two-digit numbers 10-99 = 90 pages, 
    the remaining pages from 100-589 = 490 pages, are three-digit numbers.
    Total decimal digits = 9x1 + 90x2 + 490x3 =1659
    
(8). In Lecture 6 we gave a recursive algorithm for solving the Tower of Hanoi puzzle. 
Assume we have a tower of 24 disks to move, and each move (moving one disk from one peg to another) takes one minute. The total time taken will be:
     Moves =2^n-1
     2^24-1=16777216
     one year we have 525600 minutes.
     Therefore time in years = 16777216/525600 = 31.920121765601217656012176560122 = 32 years (approx)
     
(9）.What does the following recursive function do? You may assume that the input n is always greater than 10.
     
     function f(n)
    if n >= 2 then
        return f(n-2) * n
    return 2
    It calculates 2 times the product of all odd or even integers between 1 and n 
    
(10). Which one best describes the complexity (number of basic operation executions) of the following function?
     
     function f(A[0..n-1], k)
    if n < 1 then
        return 0
    if A[n-1] == k then
        return 1 + f(A[0..n-2], k)
    return f(A[0..n-2], k)
     
     basic operation= Θ（n）
     
     
     
     
     
     
     
     
     
     
     
