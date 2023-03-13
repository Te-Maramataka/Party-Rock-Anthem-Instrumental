This README is added after the conclusion of the Hackathon by the organizer

## Party-Rock-Anthem-Instrumental
idk how this repositary thing works but here is a doc with all our stuff on it :) https://docs.google.com/document/d/1Ins0CAxPO66V6BqzPae_sKzvEopi2PU7USjwKZpFdWw/edit


- Scratch Program : https://scratch.mit.edu/projects/716759683/editor/
- Video : https://youtu.be/amXhdnrIIgs
- Screenshot at 00:10

100 Dates: 
Input Year:
Output Date:
1990
22nd June
2000
23rd June
2010
2nd July
2020
17th July
2030
21st June
2040
6th July
2050
15th July
2060
25th June
2070 -
4th July
2080
12th July
2090
23rd June
2100 -
2nd July
2110
11th July
2120
21st June
2130
30th June
2140
8th July
2150
19th June
2160
27th June
2170
6th July


2180
23rd June
2190
25th June
2200
4th July
2210
22nd June
2220
23rd June
2230
2nd July
2240
10th July
2250
21st June
2260 -
30th June
2270
15th July
2280
18th June
2290 -
4th July
2300
13th July
2310
24th June
2320 -
2nd July
2330
11th July
2340
21st June
2350
30th June
2360
8th July
2370
19th June


2380
27th June
2390
6th July
2400
23rd June
2410
25th June
2420
3rd July
2430
21st June
2440
22nd June
2450
1st July
2460
9th July
2470
20th June
2480
28th June
2490
14th July
2500
18th June
2510 -
4th July
2520
12th July
2530
23rd June
2540 -
1st July
2550
10th July
2560
20th June
2570
29th June


2580
7th July
2590
18th June
2600
27th June
2610
6th July
2620
23rd June
2630
25th June
2640
3rd July
2650
21st June
2660
22nd June
2670
1st July
2680
9th July
2690
20th June
2700 -
30th June
2710
15th July
2720
18th June
2730 -
4th July
2740
12th July
2750
23rd June
2760 -
1st July
2770
10th July


2780
20th June
2790
29th June
2800
7th July
2810
18th June
2820
26th June
2830
5th July
2840
22nd June
2850
24th June
2860
2nd July
2870
11th July
2880
21st June
2890
30th June
2900
9th July
2910
20th June
2920
28th June
2930
7th July
2940
24th June
2950
26th June
2960
11th July
2970
22nd June


2980
30th June
2990
9th July


Documentation:

Our code is really cool
We used scratch which is a great user friendly thing. ALl you need is a web browser and boom. 

Our code works by firstly finding how many days between June 19th of the year they input and Jan 1st of 1800. We Mod this day by how many days are in the lunar cycle and then add days to find the Tangaroa period. We then find the closest Friday based on this date. 

We worked great as a team and collaborated well, sharing the work evenly. Since we used scratch it was difficult to collaborate on the work as only one person could edit the code at a time. So instead what we did was hop on a discord call, screen share, and then talk to each other about our ideas on how we could change/improve the code. It wasn’t easy to find times when we could all work on it in the holidays, however after the holidays, we got cracking and together we managed to produce a functional scratch program.

Laters Gators.



RESEARCH/PLANNING:

https://www.mbie.govt.nz/assets/matariki-dates-2022-to-2052-matariki-advisory-group.pdf

^Method for finding the date of the Matariki Public holiday (always on a friday) 

Lunar month of pipiri (~ June)
There are either 12 months, each lasting 29.53 days or 13 months made up of 28 days
Tangaroa period (23rd, 24th, 25th, and 26th night)
Closest friday

The Matariki holiday always lands on a friday in either late june or early july, there is seemingly no correlation between these dates

We can’t use the 13 months of 28 days because It just wouldn’t work, trust me bro

The tangaroa lunar period DOES seem to have a correlation, we firstly need to find this correlation and create an algorithm to find it.

Looks like it repeats every 11 years however is slightly thrown off by leap days as well as the last day of the year (because 365 isn’t a multiple of 7)

For a year we can use 365.25 days, if its a decimal place we round down. (This doesn’t account for not having leap years every 100 years - exception every 400 years -)

Latest 21st of july
Earliest 19th of June

384 days between the first day of the Tangaroa lunar period 2022 and 2023 #
355 days between the first day of the Tangaroa lunar period 2023 and 2024 *
355 days between the first day of the Tangaroa lunar period 2024 and 2025 *
384 days between the first day of the Tangaroa lunar period 2025 and 2026 #
354 days between the first day of the Tangaroa lunar period 2026 and 2027 *
384 days between the first day of the Tangaroa lunar period 2027 and 2028 #
354 days between the first day of the Tangaroa lunar period 2028 and 2029 *
354 days between the first day of the Tangaroa lunar period 2029 and 2030 *
383 days between the first day of the Tangaroa lunar period 2030 and 2031 #
355 days between the first day of the Tangaroa lunar period 2031 and 2032 *
355 days between the first day of the Tangaroa lunar period 2032 and 2033 *
384 days between the first day of the Tangaroa lunar period 2033 and 2034 #
355 days between the first day of the Tangaroa lunar period 2034 and 2035 *
384 days between the first day of the Tangaroa lunar period 2035 and 2036 #
354 days between the first day of the Tangaroa lunar period 2036 and 2037 *
354 days between the first day of the Tangaroa lunar period 2037 and 2038 *
383 days between the first day of the Tangaroa lunar period 2038 and 2039 #
354 days between the first day of the Tangaroa lunar period 2039 and 2040 *
385 days between the first day of the Tangaroa lunar period 2040 and 2041 #
…


1, 3 2 3 3 2 3 2 4 2 3 3


Starting from 1 as January 1st 0000
June 19th is the 169th day of the year (170th on a leap year)

Psuedocode planning (very small)

DECLARE Year : INTEGER
DECLARE TotalDays : INTEGER
DECLARE LeapDays : INTEGER

INPUT “Input a year”, Year
LeapDays ← Year / 4

Total Days ← Year x 365

The rising of Matariki in the morning sky is observed in the month of Pipiri (around June and July). Māori wait until the lunar phase of Tangaroa, the last quarter phase of the moon
