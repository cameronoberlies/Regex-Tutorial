# RegEx Tutorial

RegEx, short for Regular Expression, is a sequence of characters that defines a search pattern. It is a powerful tool used in programming and text processing to match, search, and manipulate strings based on specific patterns.

A regular expression consists of a combination of normal characters, such as letters and digits, and special characters, which define rules and patterns to be matched within a given text. 

## Summary

This is an example of a regular expression that matches email addresses
`/^[\w.-]+@[\w.-]+\.[\w]{2,}$/`

- `[\w.-]+` matches one or more occurrences of characters that are either word characters, dots, or hyphens. This part represents the username portion of an email address. "w" is used in RegEx to match a word character

- "@" matches the "@" symbol in the email address.

- `[\w.-]+` again matches one or more occurrences of characters that are either word characters, dots, or hyphens. This part represents the domain name in an email address (like gmail, outlook etc...).

- "\." matches the literal dot (period).

- `[\w]{2,}` matches two or more word characters. This part represents the domain (.com for example) in an email address.


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

The question mark quantifier ? denotes that the preceding element is optional and can occur zero or one time. It matches the element if it occurs 0 times or once. For example, `colou?r` matches both "color" and "colour".

### <a name = "or-operator"></a>OR Operator
 The OR operator allows you to specify multiple alternative patterns or options. It enables you to match one pattern out of several possibilities. The OR operator is denoted by the pipe symbol |.

 `'example1|example2'` : Matches either `'example1'` or `'example2'`

### <a name = "character-classes"></a>Character Classes
Character classes are used to define a set of characters that can be matched at a specific position in a string.
For example, you can use \d to match any digit `(0-9)`, or `\w` to match any alphanumeric character `(a-zA-Z0-9)`.

### <a name = "flags"></a>Flags
Flags are used to modify the behavior of the pattern matching process. They allow you to change how the regex behaves, such as making it case-insensitive (Case-insensitive flag (i)) or allowing it match on multiple lines (Multiline flag (m))

### <a name = "grouping-and-capturing"></a>Grouping and Capturing
Grouping: Parentheses ( ) are used to create groups within a regular expression. Any pattern enclosed within parentheses is treated as a single unit.

Capturing: Capturing is the process of extracting the matched portion of a string that corresponds to a specific group within a regular expression. For example, the regex `\d{2}-\w+` can be used to capture the first two digits and the rest of the alphanumeric characters into separate groups.

### <a name = "bracket-expressions"></a>Bracket Expressions
Bracket expressions are enclosed within square brackets [ ] and allow you to specify a range or a group of characters that can be matched at a specific position in the input string. For example `[0-9]`: Matches any single digit from 0 to 9 or `[abc]`: Matches any single character that is either "a", "b", or "c".

### <a name = "greedy-and-lazy-match"></a>Greedy and Lazy Match
 By default, quantifiers in regular expressions are greedy which means they try to match as much of the input string as possible while still allowing the pattern to match. Lazy matching is the opposite of greedy matching. It matches as little as possible while still allowing the overall pattern to match. It is denoted by appending a ? after the quantifier. For example, the greedy `h.+l` matches 'hell' in 'hello' but the lazy `h.+?l` matches 'hel'

### <a name = "boundaries"></a>Boundaries
Similar to anchors, boundaries are special characters that match specific positions within the input string, rather than matching actual characters. They are used to define the location or context of a pattern within the string.

### <a name = "back-references"></a>Back-references
Back-references allow you to refer back to previously matched groups. For example, if you wanted to match all words that start with “a” and end with “s”, but also have the same middle characters, you could use `^(a\w+s)\1$`.

### <a name = "look-ahead-and-look-behind"></a>Look-ahead and Look-behind
Look-aheads and look-behinds allow you to check for a certain pattern before or after the main expression without actually including it in the match. For example, if you want to match all instances of the word “apple” that appear before the phrase “is tasty”, you could use `(?<=apple)\sis\stasty`
 
## <a name = "author"></a>Author

RegEx tutorial by Cameron Oberlies. Site used https://www.variables.sh/what-is-regex/#:~:text=Regexes%20are%20composed%20of%20several,classes%2C%20quantifiers%2C%20and%20alternation.

GitHub: https://github.com/cameronoberlies/Regex-Tutorial
