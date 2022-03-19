# Regex for Hex Value -

Introductory paragraph (replace this with your text)

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions) dr
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors

^ and $
^The        matches any string that starts with The 
end$ matches a string that ends with end
^The end$ exact string match (starts and ends with The end)
roar matches any string that has the text roar in it

### Quantifiers

{}
abc{2} matches a string that has ab followed by 2 c
abc{2,} matches a string that has ab followed by 2 or more c
abc{2,5} matches a string that has ab followed by 2 up to 5 c

### OR Operator

| or []
a(b|c) matches a string that has a followed by b or c (and captures b or c)
a[bc] same as previous, but without capturing b or c

### Character Classes

Not applicable

### Flags

A regex usually comes within this form /abc/, where the search pattern is delimited by two slash characters /. At the end we can specify a flag with these values (we can also combine them each other):

m (multi-line) when enabled ^ and $ will match the start and end of a line, instead of the whole string

### Grouping and Capturing

()
a(bc) parentheses create a capturing group with value bc
a(?:bc)\* using ?: we disable the capturing group
a(?<foo>bc) using ?<foo> we put a name to the group

### Bracket Expressions

[]
[abc] matches a string that has either an a or a b or a c -> is the same as a|b|c
[a-c] same as previous
[a-fA-F0-9] a string that represents a single hexadecimal digit, case insensitively
[0-9]% a string that has a character from 0 to 9 before a % sign
[^a-za-z] a string that has not a letter from a to z or from A to Z. In this case the ^ is used as negation of the expression

/^#?([a-f0-9]{6}|[a-f0-9]{3})$/

### Greedy and Lazy Match

{} - greedy operator so they expand the match as far as they can through the provided text.
? - to make it lazy

### Boundaries

Not applicable

### Back-references

Not applicable

### Look-ahead and Look-behind

Not applicable

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)

Jill Cunningham is a rising web developer. Feel free to utilize the contact details below to learn more!
Author: Jill Cunningham
Email: jleighcunningham@gmail.com
GitHub profile: https://github.com/jlcunningham2101
