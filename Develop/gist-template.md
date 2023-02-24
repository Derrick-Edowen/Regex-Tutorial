# Regular Expressions: Matching an Email

This gist tutorial with review regular expressions. Specifically the matching an email  regex. Regular expressions are used when a user wants to match a patterned  character  combination in a string.

## Summary
Match Email Regex Example - 
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
The example code above demonstates the format of a regex that is used to match and verify the format of an email address.


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
An anchor is used to determine the start and end of the string. In the expression above even though the string begins and ends  with [/] , the start is indicated by [^] and ends with [$]. Without these 2 symbols denoting the start and end, it would not be considered a match.
### Quantifiers
The quantifier for this expression is [+] . This  quantifier means that string must contain 1 or more of the previos  strings in  order for it to be considered a match. In the case of this string ^([a-z0-9_\.-]+), any string containing a-z,0-9,_\.- can be a match.
### OR Operator
The OR operator | is not used in the matching email regex. However the OR operator this operator denotes that there is variation possible in a string. As seen  in the Hex Value regex  /^#?([a-f0-9]{6}|[a-f0-9]{3})$/,  there can be [a-f0-9]{6} or [a-f0-9]{3} in a string  to still  have a match.
### Character Classes
The character class found in /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ is [\d] and [a-z]. This character classindicates  any digit can be used in its place and  will still have a match. Digits are considered and  value from 0-9. [\da-z\.-]+ this section  of the regex means a letter from a-z and digit from 0-9 can be used in the string.
Other Classes:
"\d" represents digits
"\D" represents not digits
"\w" repesents words
"\W" represents not words
"\s" represents whitespace
"\S" represents not whitespace
"[abc]" represents a,b, or c
"[^abc]" represents not a,b, or c
"[a-z]" represents any letter from a -z
### Flags
The Email regex does not include a flag.
Other flags that can be found in other regexs:
"i" - stands for insensitive. This flag is used  to ignore where the string is a capital case or lower case.
"g" - Makes the expression search for all occurrences
"s" - Makes the wild character . match newlines as well
"m" - changes  boundary of [^] and [$] anchors to every line rather than entire string
### Grouping and Capturing
Group in the email  matching regex is denoted with parentheses [()]. /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
this regex contain 3 groups all separated by parentheses with similar character classes within the group.
Group 1: ([a-z0-9_\.-]+)
Group 2: ([\da-z\.-]+)
Group 3: ([a-z\.]{2,6})
### Bracket Expressions
Bracket expressions are used to denote a list  of characters/classes that can only be used in that group. For example [a-z0-9_\.-] has a bracket  expression that contains specific string requirements. In the group above it is a-z, 0-9, and certain special characters.
### Greedy and Lazy Match
This regex does not conatin a greedy or lazy match quantifier. The greedy indicates the  longest possible string, while lazy indicates the shortest possible string. Email match does not make  consideration for the  length of the result.
### Boundaries
Boundaries are not present in the email regex. Boundaries are denoted  by [\b] and can be used to isolate words. [\b] searches and analyzes entire words and  can be used for many purposes  such as isolating letters in words.
### Back-references
Back references are denoted using [\]. They are used to identify previous groups that match and looks for the same string again. Back references are not present in this regex.
### Look-ahead and Look-behind
Look-ahead and look-behind is not  present in this regex. The function of look-ahead and look-behind are to determine what immediately follows and preceds a current position in a string. Can be used to validate certain characters in a string.
Example: 
Look-ahead - [?=]
look-behind - [?<=]
## Author
Derrick Edowen,  currently enrolled in UofT coding bootcamp  full-stack developer course.
Github - [https://github.com/Derrick-Edowen]
