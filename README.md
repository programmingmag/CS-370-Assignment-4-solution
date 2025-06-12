# CS-370-Assignment-4-solution

Download Here: [CS 370 Assignment 4 solution](https://jarviscodinghub.com/assignment/cs-370-assignment-4-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

1. (10 marks) Find the P A = LU factorization by hand using row pivoting with maximal pivot
for the following matrix:
A =


2.0 1.0 4.0
−4.0 −2.0 6.0
1.0 1.0 2.0

 .
Use this factorization to solve Ax = b where
b =


2.0
1.0
9.0

 .
2. (20 marks) Computing a natural spline with interpolation points having ∆xi equal for all i
requires solving a linear system A~x = ~b where
A =












2 1 0 · · · 0 0
1 4 1 0 0
0 1 4 1 0 0
.
.
.
.
.
.
.
.
.
.
.
.
.
.
.
.
.
.
0 0 0 1 4 1
0 0 0 1 2












n×n
and ~x is the vector of derivatives of the spline. In this question you will investigate the
solution of the linear system and determine its cost.
(a) The factors of A = LU have the form
L =









1 0 · · · 0 0
l2 1 0 0
0 l3 1
.
.
.
.
.
.
0 0 1 0
0 0 ln 1









U =









d1 u1 · · · 0 0
0 d2 u2 0
0 0 d3 u3
.
.
.
.
.
.
0 0 dn−1 un−1
0 0 0 dn









Find the recurrence equations which determine li
, di and ui
.
(b) What is the cost (that is, O(n
k
), for some k) of finding an LU decomposition of A?
Justify your answer.
(c) What would the cost be to compute a natural spline when all the ∆xi are the same?
1
3. (20 marks) Consider the small web given by
The probabilities displayed are the output of the pagerank algorithm for α = 0.85. You can
use these to check the correctness of your pagerank algorithm.
(a) Construct the Google matrix M for this web.
(b) Run the PageRank algorithm for 15 iterations to find a ranking vector ~x. Use α = 0.75.
(c) Verify that the ranking vector ~x approximately satisfies M~x = ~x.
You can use either Maple or Matlab for this question.
4. (10 marks) A matrix Q = [qij ] is a positive Markov matrix if 0 < qij < 1 and P i qij = 1. Show that the Google matrix M = α(P + 1 R e dT ) + (1 − α) 1 R e eT is a positive Markov matrix. 5. (15 marks) Consider the positive n × n positive Markov matrix M, having n linearly independent eigenvectors xi , associated with eigenvalues λi . The PageRank algorithm uses the iteration p k+1 = Mp k , (1) with p ∞ = lim k→∞ (M) kp 0 . (a) Show that Xn `=1 [p k+1]` = Xn `=1 [p k ]` . 2 (b) If x = [x1, · · · , xn] T P is the unique eigenvector of M corresponding to λ = 1, show that n i=1 xi 6= 0. 6. (25 marks) (a) Write a function function [p, iter] = MyPageRank(G, alpha) to compute the pagerank using the algorithm in Section 7.7 of the course notes. The inputs are the connectivity matrix G and the weight α. The output is the vector p of page ranks, and iter is the number of iterations that were required for the computation. Use a tolerance value of 10−7 . Note: Let Gij denote the (i, j)-th entry of the matrix G. Gij = 1 indicates that there is a link from j to i. Gij = 0 indicates no such link. Note: You must take advantage of the sparsity of G. Avoid using additional loops (within the iteration loop) or creating full matrices (see Section 7.6 in the course notes). (b) Run your code on the following small web using α = 0.75: (c) A connectivity matrix G and a list of URLs are provided in math uwaterloo.mat. The data represents a network of 500 pages and was generated starting from the website math.uwaterloo.ca. Load the data and compute the pageranks with α = 0.85. Use the following code to obtain the final ranking order and list the top twenty results: [y I] = sort(p, ’descend’); for n = 1:min(length(I), 20) disp([num2str(n) ’: ’ U{I(n)}]); end (d) Experiment with the math uwaterloo.mat using the following values of α: 0.15, 0.6, 0.75, 0.95. Report the number of iterations in each case. What do you notice about the relationship between α and the number of iterations? Explain.

