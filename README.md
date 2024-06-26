# Mutual_friends
Pyspark problem to find mutual friends from the given .txt file 

Problm: Finding Common Friends with Spark

Input:
A text file named "friends.txt" with lines in the format: person_id<TAB>friend1,friend2,friend3,...

Output:
A list of tuples, where each tuple contains a pair of people IDs and the list of their common friends.

Sample Input: friends.txt
1	2,3,4
2	1,3,5
3	1,2,5
4	1,5
5	2,3,4

Sample Output -

[("1", "2", ["3", "4"]), ("1", "3", ["2"]), ("2", "3", ["1"]), ("1", "4", ["5"]), ("1", "5", []), ("2", "5", ["3"]), ("3", "5", ["2"])]

Explanation:

This code is a Spark application written in Python that processes a file containing a social network's adjacency list (friend list) and generates a list of mutual friends between each pair of users. Here’s a detailed explanation of the code
