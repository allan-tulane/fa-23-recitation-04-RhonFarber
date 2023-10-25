# CMPS 2200 Reciation 5
## Answers

**Name:**Rhon Farber


Place all written answers from `recitation-05.md` here for easier grading.


- **1b.**
Sorted:

|   n |   qsort-fixed-pivot |   qsort-random-pivot |
|-----|---------------------|----------------------|
|  10 |               0.086 |                0.061 |
|  50 |               0.780 |                0.349 |
| 100 |               2.701 |                1.087 |
| 200 |              10.109 |                2.189 |
| 300 |              82.840 |                5.754 |
| 400 |             103.612 |                6.105 |
| 450 |             195.379 |                4.680 |
| 500 |             103.561 |                4.512 |
| 600 |             110.183 |                3.484 |
| 700 |             186.152 |                8.015 |

Unsorted:
|   n |   qsort-fixed-pivot |   qsort-random-pivot |
|-----|---------------------|----------------------|
|  10 |               0.083 |                0.074 |
|  50 |               0.237 |                0.278 |
| 100 |               0.306 |                0.487 |
| 200 |               1.343 |                1.765 |
| 300 |               2.906 |                2.831 |
| 400 |               2.070 |                2.700 |
| 450 |               2.165 |                2.989 |
| 500 |               2.445 |                3.630 |
| 600 |               2.625 |                2.952 |
| 700 |               3.126 |                3.977 |

Using a fixed pivot on a sorted list proves to be highly inefficient, particularly as the size of the input grows. This is understandable since choosing the initial element as the pivot in a sorted list isn't effective for dividing the list into sub-arrays, causing the algorithm to operate in an inefficient manner (essentially processing one element at a time). Although the observed runtimes might seem similar, employing a random list or a random pivot clearly demonstrates better efficiency.

- **1c.**
Sorted:

|   n |   qsort-fixed-pivot |   qsort-random-pivot |   tim_sorted |
|-----|---------------------|----------------------|--------------|
|  10 |               0.069 |                0.042 |        0.003 |
|  50 |               0.667 |                0.399 |        0.005 |
| 100 |               3.010 |                0.667 |        0.008 |
| 200 |              12.787 |                1.651 |        0.012 |
| 300 |              77.369 |                2.387 |        0.007 |
| 400 |              81.232 |                6.004 |        0.011 |
| 450 |             103.833 |                3.790 |        0.011 |
| 500 |             112.669 |                5.435 |        0.009 |
| 600 |             105.304 |               48.049 |        0.022 |
| 700 |             136.841 |                3.486 |        0.011 |

Unsorted:
|   n |   qsort-fixed-pivot |   qsort-random-pivot |   tim_sorted |
|-----|---------------------|----------------------|--------------|
|  10 |               0.060 |                0.061 |        0.005 |
|  50 |               0.251 |                0.331 |        0.007 |
| 100 |               0.606 |                0.681 |        0.017 |
| 200 |              52.806 |                1.510 |        0.031 |
| 300 |               1.453 |                2.180 |        0.043 |
| 400 |               2.249 |                3.917 |        0.063 |
| 450 |               6.933 |               13.312 |        0.083 |
| 500 |               5.430 |                5.332 |        0.077 |
| 600 |               3.373 |                4.195 |        0.072 |
| 700 |               2.921 |                3.760 |        0.117 |

Tim Sort significantly outperforms the other algorithms. It has the quickest execution times, irrespective of the list being sorted or shuffled.