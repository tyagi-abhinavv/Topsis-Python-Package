---
---
---

# **Topsis-Abhinav-102067004**

| This library has been created as a part of the assignment for UCS654. This package implements Technique for Order of Preference by Similarity to Ideal Solution(TOPSIS) for solving Multiple Criteria Decision Making(MCDM) problems.

### **Installation**

| This package can be installed using pip package manager

<div>

pip install Topsis-Abhinav-102067004

</div>

### **Usage**

| The library provides support for a 'topsis' command which can be invoked through the command line
| ***Input Arguments:***

-   file: a file with '.csv' extension, which should only have numeric values for all features, beyond the second column. This file should have minimum three columns, otherwise an error would occur

-   weights: A numeric array, with weights value for each feature column

-   impacts: A character array with '+' corresponding to features with positive impact and '-' corresponding to features with negative positive impact

-   output file name: name of the output csv file having TOPSIS score and rank columns appended to the input file

| ***Output:***
| The result table will be printed to the console and a csv file will be created with the output file name

### **Example**

| **file.csv**

| Fund Name | P1   | P2   | P3  | P4   | P5    |
|-----------|------|------|-----|------|-------|
| M1        | 0.67 | 0.45 | 5.1 | 66.4 | 18.16 |
| M2        | 0.8  | 0.64 | 4.9 | 46.7 | 13.26 |
| M3        | 0.68 | 0.46 | 3.6 | 34.9 | 9.91  |
| M4        | 0.84 | 0.71 | 4.7 | 36.8 | 10.76 |
| M5        | 0.68 | 0.46 | 4.7 | 51.1 | 14.24 |
| M6        | 0.63 | 0.4  | 5.3 | 54.5 | 15.21 |
| M7        | 0.8  | 0.64 | 3.7 | 67.3 | 18.11 |
| M8        | 0.79 | 0.62 | 3.3 | 66.6 | 17.83 |

| Weights = [1,1,1,1,1]
| Impacts = ['+', '+', '+', '+', '-' ]

<div>

topsis input.csv 1,1,1,1,1 +,+,+,+,- output.csv

</div>

#### **Output**

| **To console:**

<div>

Results:

Fund Name P1 P2 P3 P4 P5 Topsis Score Rank

0 M1 0.67 0.45 5.1 66.4 18.16 0.484608 5.0

1 M2 0.8 0.64 4.9 46.7 13.26 0.605915 1.0

2 M3 0.68 0.46 3.6 34.9 9.91 0.396911 8.0

3 M4 0.84 0.71 4.7 36.8 10.76 0.596375 2.0

4 M5 0.68 0.46 4.7 51.1 14.24 0.440537 7.0

5 M6 0.63 0.4 5.3 54.5 15.21 0.445909 6.0

6 M7 0.8 0.64 3.7 67.3 18.11 0.53706 3.0

7 M8 0.79 0.62 3.3 66.6 17.83 0.507571 4.0

</div>

| **outputfilename.csv:**

| Fund Name | P1   | P2   | P3  | P4   | P5    | Topsis Score | Rank |
|-----------|------|------|-----|------|-------|--------------|------|
| M1        | 0.67 | 0.45 | 5.1 | 66.4 | 18.16 | 0.484607532  | 5    |
| M2        | 0.8  | 0.64 | 4.9 | 46.7 | 13.26 | 0.605914538  | 1    |
| M3        | 0.68 | 0.46 | 3.6 | 34.9 | 9.91  | 0.396910752  | 8    |
| M4        | 0.84 | 0.71 | 4.7 | 36.8 | 10.76 | 0.596374527  | 2    |
| M5        | 0.68 | 0.46 | 4.7 | 51.1 | 14.24 | 0.44053701   | 7    |
| M6        | 0.63 | 0.4  | 5.3 | 54.5 | 15.21 | 0.445909442  | 6    |
| M7        | 0.8  | 0.64 | 3.7 | 67.3 | 18.11 | 0.537060234  | 3    |
| M8        | 0.79 | 0.62 | 3.3 | 66.6 | 17.83 | 0.507571147  | 4    |

### **License**

MIT
