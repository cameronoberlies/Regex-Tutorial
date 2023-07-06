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
- [Author](#author)


## Regex Components


### <a name = "anchors"></a>Anchors
Anchors are used to match the starting and ending points of a string or line. The "^" symbol is used to match the beginning and the "$" symbol to match the end of a string.

### <a name = "quantifiers"></a>Quantifiers
Quantifiers are used to specify the quantity or repetition of the preceding character or character class. They allow you to define how many times a particular character, group, or character class should appear in the input string. Quantifiers are typically placed immediately after the element they apply to. For example, you can use * to match zero or more occurrences of the preceding character or character class, or + to match one or more occurrences of the preceding character or character class. 

The question mark quantifier ? denotes that the preceding element is optional and can occur zero or one time. It matches the element if it occurs 0 times or once. For example, colou?r matches both "color" and "colour".

### <a name = "or-operator"></a>OR Operator
 The OR operator allows you to specify multiple alternative patterns or options. It enables you to match one pattern out of several possibilities. The OR operator is denoted by the pipe symbol |.

 'example1|example2' : Matches either 'example1' or 'example2'

### <a name = "character-classes"></a>Character Classes
Character classes are used to define a set of characters that can be matched at a specific position in a string.

### <a name = "flags"></a>Flags

### <a name = "grouping-and-capturing"></a>Grouping and Capturing

### <a name = "bracket-expressions"></a>Bracket Expressions

### <a name = "greedy-and-lazy-match"></a>Greedy and Lazy Match

### <a name = "boundaries"></a>Boundaries

### <a name = "back-references"></a>Back-references

### <a name = "look-ahead-and-look-behind"></a>Look-ahead and Look-behind

## <a name = "author"></a>Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
