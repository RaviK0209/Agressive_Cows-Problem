# Agressive_Cows-Problem
Python code :-Placing number of cows in given number of stalls within minimum largest possible distance between them.
<br>
PROBLEM:-There is a new barn with N stalls and C cows. The stalls are located on a straight line at positions x1,xN (0 <= xi <= 1,000,000,000).
         We want to assign the cows to the stalls, such that the minimum distance between any two of them is as 
         large as possible. What is the largest minimum distance?
 <BR>
ALGORITHM TO SOLVE TYHE ABOVE PROBLEM:-
 1.	Sort the Stalls: [1,2,,4,8,9]
 2.	Binary Search Range: Start with low = 0 and high = 8 (distance between the first and last stall).
 3.	First Mid-point: 4 (check if you can place cows with at least 4 units apart).
 	      Place the first cow at 1.
  	      The next cow can go at 8 (since 8 - 1 >= 4).
 	      The third cow can go at 9 (since 9 - 8 >= 4).
 	All cows are placed, so 4 is feasible. Try a larger distance.
 4.	Next Mid-point: 6 (check if you can place cows with at least 6 units apart).
 	      Place the first cow at 1.
 	      The next cow can go at 8 (since 8 - 1 >= 6).
 	       Only 2 cows are placed, so 6 is not feasible. Try a smaller distance.
 5.	Adjust Range: Continue adjusting and checking until you find the largest feasible minimum distance, which will be 3 in this case.
