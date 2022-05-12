# Email-Regex

This tutorial will explain the of use the regex that helps you validate emails.
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Summary
An expression is a sequence of characters that assist the user to validate input based on the patterns.

## Table of Contents
- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)
- [OR Operator](#or-operator)

## Regex Components

### Anchors
^ The anchors are used for matching emails and are the start of the expression. $ Closes the expression

### Quantifiers
+, connects the users email name, email service & .com. 
{2,6}, allows a matching range of 2-6 for the set [a-z\.].

### Character Classes
\d matches a single character that is a digit from 0-9. 
It will only match one specific character.

### Flags
Regular expressions may have flags that affect the search:
d 
Generate indices for substring matches.

### Grouping and Capturing
Group 1([a-z0-9_\.-]+) matches email address. 
Group 2([\da-z\.-]+) matches company services.
Group 3([a-z\.]{2,6}) captures the .com/.net/.org.

### Bracket Expressions
[a-z0-9_\.-] use for email validation and it matches the characters a-z, 0-9,"_" , "-" , and "."
[\da-z\.-], which is matching a single digit from 0-9, any character a-z (case senstive), and the "." and "-"
[a-z\.] matches any character a-z(case senstive) and the character ".".

### Greedy and Lazy Match
+ Quantifier, it will match as many times as possible giving back as needed. 
{} Another greedy Quantifier used in this regex is  when matching `{2,6} for the last capture group.

### Boundaries
\b There's three boundaries in a string: at the beginning, the end and in between two charaters.

### Back-references
\1 Matches same text which was previously matched in a group.

### Look-ahead and Look-behind
They're also known as "lookarounds" have no boundaries and will start looking if there's a match or not.

### OR Operator
| or \ Will match one of the choices in the sequence. 

## Author
https://gist.github.com/rakky21