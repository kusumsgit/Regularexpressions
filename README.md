## Regular Expressions
Regular expression are very useful in extracting information from text such as code, log files, spreadsheets, or even documents. 
1. Letters abc etc.
2. \d can be used in place of any digit from 0 to 9.
3. Period (.) can match any single character (letter, digit, whitespace, everything). To skip periof we use \.
3. [abc] will match a, b or c. Matching specific characters by defining them inside square brackets.
4. [^abc] will match any single character except for the letters a, b, or c.
5. [A-E] [a-c] [0-4] or [^A-E] [^a-c] [^0-4] is used to match or not match a single character between the range mentioned in square brackets. It is case sensitive.
6. a{3} or b{3,5} it shows repetition of a 3 times and b 3 to 5 times. .{2,6} means repetition of any character 2 to 6 times.
7. \w any Alphaneumeric 
8. \W any non-alphanumerc
9. The symbol (*) Zero or more repetition
10. They symbol (+) one or more repetition
11. ? This metacharacter allows you to match either zero or one of the preceding character or group. To skip ? use \?
12. \s any whitespace character
13. \S any non-whitespace character
14. ^ (hat) and $ (dollar) sign to match the starting and end of the line. ^ is different than [^]
15. () captures group and (a(bc)) captures subgroup example of capturing groups and subgroups is below. 

|Text|Capture Groups|
|------|------------|
|Capture	Jan 1987	 |  Jan 1987 1987	|
|Capture	May 1969	 | May 1969 1969	|
|Capture	Aug 2011	 |  Aug 2011 2011 |

Answer: (\w+\s*(\d+)) : \w+  for any alphaneumeric character repeated one or more time then \s* for whitespace used zero or more times 
and \d+ means any digit for 1 or more times.

17. (.*) capture all

18. | pipe is used for as an OR logical expression
