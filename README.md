## Description of LCuS

LCuS.py is a naive O(n^5) approach to solving the longest cubic subsequence 
(LCuS) problem. 

For a string of characters, LCuS.py identifies the longest subsequence repeated 
three distinct times. It finds the optimal breakpoints to seperate the string 
into three consecutive substrings, each containing an interation of the 
subsequence. It then returns these indices and three matrices, F, D, and E. For given (valid) values of j, l, m, for all i in the range (1,...,j-1) and all k in the range (j,...,l-1):

* the F matrix holds values all f(i, k) 
* the D matrix holds values all d(i, k)
* the E matrix holds values all e(i, k)

For more information, see paper (* citation)

## Requirements

1. Install python 3.12 or higher
2. Use Conda or other similar environment to run NumPy package:
(https://www.numpy.org)

## Running LCuS

Clone the repository: 
```
$ git clone https://github.com/robynburger/LCS_naieve
```

Run LCuS.py:
```
$ python LCuS.py
```

Enter command line arguments:
```
Enter string:

Use ideal parameters? (Yes/No):
```
If user types 'Yes:
``` 
Your file was saved: results/s/ideal.txt
```
If user types 'No':
```
Enter positive integers j, l, m:

Note: 1 <= i < j <= k < l <= m <= {len(s)}.

j:

l:

m:

Your file was saved: results/s/j_l_m.txt
```

## Authors and Acknowledgements 

Written by Robyn Burger and Allison Shi under the mentorship of 
Dr. Brendan Mumey and Dr. Adiesha Liyanage. 

Funded by the National Science Foundation (NSF) as part of research conducted 
at Montana State University for the summer 2024 Algorithms REU. 

Adapated from longest tandem subsequence problem:   

Kosowski, Adrian., An Efficient Algorithm for the Longest Tandem
Scattered Subsequence Problem,  Lecture Notes in Computer Science, volume 3246 
(2004) 93-100.
