# RegEx Tutorial

RegEx, short for Regular Expression, is a sequence of characters that defines a search pattern. It is a powerful tool used in programming and text processing to match, search, and manipulate strings based on specific patterns.

A regular expression consists of a combination of normal characters, such as letters and digits, and special characters, which define rules and patterns to be matched within a given text. 

## Summary

This is an example of a regular expression that matches email addresses
/^[\w.-]+@[\w.-]+\.[\w]{2,}$/

- "[\w.-]+" matches one or more occurrences of characters that are either word characters, dots, or hyphens. This part represents the username portion of an email address. "w" is used in RegEx to match a word character

- "@" matches the "@" symbol in the email address.

- "[\w.-]+" again matches one or more occurrences of characters that are either word characters, dots, or hyphens. This part represents the domain name in an email address (like gmail, outlook etc...).

- "\." matches the literal dot (period).

- "[\w]{2,}" matches two or more word characters. This part represents the domain (.com for example) in an email address.


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


### <a name = "anchors"></a>Anchors

### Quantifiers

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
