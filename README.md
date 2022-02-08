# HackerRank-Plus-Minus-Solution-
HackerRank warmup / plus Minus Solution

#!/bin/python3

import math
import os
import random
import re
import sys

#
# Complete the 'plusMinus' function below.
#
# The function accepts INTEGER_ARRAY arr as parameter.
#

def plusMinus(arr):
    # Write your code here
    pos = []
    neg = []
    z = []
    for i in arr:
        if i > 0:
            pos.append(i)
        elif i < 0:
            neg.append(i)
        else:
            if i == 0:
                z.append(i)
    print("{0:.6f}".format(len(pos)/len(arr)))
    print("{0:.6f}".format(len(neg)/len(arr)))
    print("{0:.6f}".format(len(z)/len(arr)))


    
            

if __name__ == '__main__':
    n = int(input().strip())

    arr = list(map(int, input().rstrip().split()))

    plusMinus(arr)

