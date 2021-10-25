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

### Character Classes
Character classes distinguish different types of characters for example, letters and numbers.
1. In this regex the `@` and `.` are two characters the regex must distinguish before validating the email.

### The OR Operator
There was not any OR operators in this regex.
### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
