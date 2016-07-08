# FP-growth
A simple implementation of the FP-growth algorithm by Jiawei Han and Jian Pei [SIGMOD 2000]

Usage: fpgrowth datafile minsup [output]

Note that minsup must not be a relative frequency, but an (absolute) natural number between 1 and the number of transactions!
All items occurring in the database must be positive integers!

Each line contains a list of items (integers) separated by white space and ended by a newline.
An empty line (ended by a newline) thus also means an empty transaction.

Output
------

The frequent itemsets are (optionally) printed in the output file
given on the command line. 
If provided, all itemsets are printed to that file together with their support.
For example:
1 2 3 (10)
means that itemset {1,2,3} occured in 10 transactions of the database.


Runtime output: 
---------------

Speaks for itself

For example: 

items read [0.12s]
items reordered and pruned [0s]
FPtree constructed [0.3s]
Frequent sets generated [0.57s]
3991    0.99

shows that 3991 frequent itemsets were generated in .99 seconds

Have fun and if you have any other question, please let me know.

Bart Goethals.
