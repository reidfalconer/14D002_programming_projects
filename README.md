# 14D002: Deterministic Models and Optimization

## Programming Projects:

## **Edit Distance**

In computer science, edit distance is a way of quantifying how dissimilar two strings are to one another by calculating the minimum number of edit operations necessary to transform one string into the other. One of the simplest sets of edit operations is that defined by Levenshtein in 1966 which consist of three operations on a string::

- I: Insertion of a character.
- D: Deletion of a character.
- S: Substitution of a character.

Each operation has an imputed cost, and subsequently the algorithm strives to minimise the cost of edit operations (i.e.the  number of operations (D , I , S).

We design an algorithm that, given two strings X and Y, computes the edit distance between X and Y. Furthermore, the algorithm  provides one with the optimal sequence of operations required to transform X into Y.

## **Huffman Codes**

Huffman coding is a lossless data compression algorithm. It assigns variable-length codes to each symbol, lengths of the assigned codes are based on the frequencies of corresponding symbols. The smallest code is assigned to the most frequent symbol and vice versa.

Prefix Codes, which the bit sequences are assigned in such a way that the code assigned to one symbol is different from any other symbols, are assigned so that Huffman Coding makes sure that there is no ambiguity when decoding the generated bitstream.

To compute this algorithm, a greedy approach is used. This technique looks at the frequency of each character at each round and stores it as a binary string in an optimal way (i.e.  at each step, the algorithm makes a "greedy" decision to merge the two subtrees with least weight).

Here we build two algorithms:
1. An algorithm that, when given an input text T, constructs an optimal prefix code for T.
2. An algorithm that, given a prefix code for a text T, outputs T.
