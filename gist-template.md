# Regular Expression Tutorial

Regular expression, also called Regex, is a sequence of characters that defines a specific pattern. When utilizing regex, they can be used to: finding a pattern of characters within a string, replace a character or series of characters within a string or to validate input.

## Summary

This tutorial will explain the regex, 
``` /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ ``` , which is utilized to verify an email address. 

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)


## Regex Components
The email validating regex utilizes the following components, which will be fully explained below: anchors, captures/groups, bracket expressions, and character classes.
### Anchors
The  ^ and $ characters are considered anchors. The ^ anchor determine a string that begins with the characters that follow it. The $ anchor works like the opposite in that it signifies a string that ends with the characters that precede it. The email regex begins with ^ and ends with the $ anchors.
### Quantifiers
Quantifiers set the limits of the string that the email regex matches. Often, they include the minimum and maximum number of characters that a regex is searching for. There are two quantifiers in the email regex: ``` ([a-z0-9_\.-]+) ``` and ``` ([a-z\.]{2,6}) ```. In the first quantifier, the + means that atleast one of the preceding characters must be matched. In the second quantifier, the numbers inside the curly braces means that the regex must match 2-6 characters it is preceding. 

### Grouping Constructs
The bigger a regex is there may be multiple parts of a string to determine that different sections satisfy different requirements. The main way to group a part of a regex is with parenthesis. The email validating regex contains three groups: ``` ([a-z0-9_\.-]+) ```,  ``` ([a-z\.]{2,6}) ```. and ```([a-z\.]{2,6})```.
### Bracket Expressions
Characters inside a set of square brackets represents the range of characters that is being matched. 
### Character Classes

### The OR Operator
The OR operator surprisingly does not stand for anything fancy - it literally means or as in, "you may have a or b". It is signified using the | symbol. The email validator does not use the OR operator.


## Author

michael montoya
