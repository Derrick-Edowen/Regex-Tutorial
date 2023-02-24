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
An anchor is used to determine the start and end of the string. In the expression above even though the string begins and ends  with / , the start is indicated by ^ and ends with $. Without these 2 symbols denoting the start and end, it would not be considered a match.
### Quantifiers
The quantifier for this expression is + . This  quantifier means that string must contain 1 or more of the previos  strings in  order for it to be considered a match. In the case of this string ^([a-z0-9_\.-]+), any string containing a-z,0-9,_\.- can be a match.
### OR Operator
The OR operator | is not used in the matching email regex. However the OR operator this operator denotes that there is variation possible in a string. As seen  in the Hex Value regex  /^#?([a-f0-9]{6}|[a-f0-9]{3})$/,  there can be [a-f0-9]{6} or [a-f0-9]{3} in a string  to still  have a match.
### Character Classes
The character class found in /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ is \d. This character classindicates  any digit can be used in its place and  will still have a match. Digits are considered and  value from 0-9. [\da-z\.-]+ this section  of the regex means a letter from a-z and digit from 0-9 can be used in the string.
Other Classes:
"\d" represents digits
"\D" represents not digits
"\w" repesents words
"\W" represents not words
"\s" represents whitespace
"\S" represents not whitespace
"[abc]" represents a,b, or c
"[^abc]" represents not a,b, or c
### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
