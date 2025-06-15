# Machine Problem 2 | Bottle Collector

Rikku is a young boy who dreams of becoming a businessman. In his spare time, he likes to go around
the city and gather empty bottles to sell to the local junk shop. He has made enough money and wants
to try investing in a programmer, being you, to create a program for calculating his earnings.

The program will require 2 inputs:
● A numeric value that represents his daily expenses for travels and meals
● An array of strings representing each day&#39;s expeditions, with each string in the format &quot;{hours}
{path} {price}”

For the strings in the input array, the format is explained as:
Hours, being the hours he spends collecting bottles on that particular day
● Path, being a sequence of letters representing his travels for that particular day, with successful
bottle findings marked as &quot;B&quot;, and any other letter as no bottle found
● Price, being the amount of money, he sells each bottle for, only for that day, assuming that the
local junk shop has different buying rates per day
For each day, Rikku will walk left to right on the path given, each letter being searched for an hour.
When he still has hours remaining and he has already reached the end of the path, he will return to the
very beginning of his path and repeat his search, somehow finding bottles again in the same areas
where he had found them before he looped back to his first area.
For example: &quot;8 ABMRB 24.50&quot; Rikku will travel for 8 hours. It takes 5 hours to loop through &quot;ABMRB&quot;,
then with 3 hours left, Rikku goes through only &quot;ABM&quot; in the second loop. There are 2 &quot;B&quot;s in &quot;ABMRB&quot;,
so Rikku gets 2 bottles from that loop. There is 1 &quot;B&quot; in &quot;ABM&quot;, so Rikku gets 1 bottle from that loop.
With 3 bottles, Rikku sells them all for 24.50 each, earning 73.50 in total for that one day.

You must get the total earnings for all his days, as well as the average earnings. If the average earnings
are greater than his daily expenses (the first input in the program), have program the return &quot;Good
earnings. Extra money per day: {average earnings - daily expenses}&quot; Otherwise, if the average earnings
are less than his daily expenses, have the program return &quot;Hard times. Money needed: {total daily
expenses - total earnings}&quot; Take note that the above &quot;total daily expenses&quot; is simply the daily expenses
multiplied by the number of elements in the array given as the second argument (the number of days he
went bottle hunting).

All numbers included in the return values must have the precision of two (2) decimals.
Examples:
Good earnings. Extra money per day: 250.67
Hard times. Money needed: 999.00
