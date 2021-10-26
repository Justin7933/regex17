# Validating Email Addresses

Regex is a short word for regular expression and it is used to detect diffrent patterns within a string. A good example of a regualr expression is validating an email address. This allows you to have a much cleaner database because, if you did not validate the email addresses people are using. It could become an issue due to the fact people could make random email addresses that have never been registered. 

## Summary

The expression for validating email addresses is `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`. Using this in your sites could come in handy almost everytime.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors
Anchors are the begining and the end of the expression.
1. ^
2. $
### Quantifiers
Quantifiers help to see how many instances must be shown for a match to be found.
1. the plus in the email expression viewed here `([\da-z\.-]+)\` allows the component to be broken up into the name, domain and TLD. Example: justin@gmail.com
2. `{2,6}` is to only find matches that are more than 2 characters and less than 6 characters.

### Grouping Constructs
The grouping in the expression can be seen by the parentheses inside the regex.
1.Email: `/^([a-z0-9_\.-]+)`
2.Domain: `@([\da-z\.-]+)\`
3. TLD: `.([a-z\.]{2,6})$/`
### Bracket Expressions
Anything with `[]` around it is considered a bracket expression. In this regex there is three.
1. `/^([a-z0-9_\.-]+)` this is to find any lowercase letter from a-z and any number from 0-9
2. `([\da-z\.-]+)\` this is to find any lowercase letter from a-z and the /d puts a number to each of those letters
3. `([a-z\.]{2,6})$/` this is to find any lowercase letter from a-z and also is looking for a period(.)
### Character Classes
Character classes distinguish different types of characters for example, letters and numbers.
1. In this regex the `@` and `.` are two characters the regex must distinguish before validating the email.

### The OR Operator
An OR operator allows the regex to do either one or the other request in the expression. In this regex you can see `([a-z0-9_\.-`. The regex is finding any lowercase letter from a-z OR any number from 0-9.
### Flags
There are no flags in this regex. A flag though is used after the second `/` in the regex. An example is `i` and it is used to ignore any case sensitive searches.
### Character Escapes

## Author
<a href="https://github.com/Justin7933" target="_blank">Github Profile</a>

