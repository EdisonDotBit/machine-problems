# Machine Problem 1

Adding parts
Let us consider this example (array written in general format):
ls = [0, 1, 3, 6, 10]

Every possible parts of the array:
ls = [0, 1, 3, 6, 10]
ls = [1, 3, 6, 10]
ls = [3, 6, 10]
ls = [6, 10]
ls = [10]
ls = []
The corresponding sums are (put together in a list): [20, 20, 19, 16, 10, 0]
The function ( part_sums / partSums / SumParts ) (or its variants in other languages) will take as
parameter a list ls and return a list of the sums of its parts as defined above.

Example:
ls = [1, 2, 3, 4, 5, 6]
parts_sums(ls) -&gt; [21, 20, 18, 15, 11, 6, 0]
ls = [744125, 935, 407, 454, 430, 90, 144, 6710213, 889, 810, 2579358]
parts_sums(ls) -&gt; [10037855, 9293730, 9292795, 9292388, 9291934, 9291504,
9291414, 9291270, 2581057, 2580168, 2579358, 0]
