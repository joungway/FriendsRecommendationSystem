# Friends Recommendation System in Python

A Spark program that implements a “People You Might Know” social network friendship recommendation algorithm: if two people have a lot of mutual friends, then the system should recommend that they connect with each other.

## 1. Data
Associate data is in the data folder, an adjacency list with the following format: <User><TAB><Friends>.

## 2. Algorithm
For each user U, the algorithm recommends N = 10 users who are not already friends with U, but have the most number of mutual friends in common with U.

## 3. Output
The output format is <User><TAB><Recommendations>, where <User> is a unique ID corresponding to a user and <Recommendations> is a comma separated list of unique IDs corresponding to the algorithm’s recommendation of people that <User> might know, ordered in decreasing number of mutual friends.


Input
The input file, contained in the 'data' folder, contains the adjacency list and has multiple lines in the following format: where is a unique integer ID corresponding to a unique user and is a comma-separated list of unique IDs corresponding to the friends of the user with the unique ID .
