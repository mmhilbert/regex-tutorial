# Title (replace with your title)

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
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors
These are special characers that allow you to specify a position in the string where the pattern should start or end. Here are examples of achors and their uses:

1. Caret (`^`)
* This asserts that the following pattern must start at the beginning of the string
* example: `^Hello` matches "Hello" only if it is at the beginning of a line or string

2. Dollar Sign (`$`)
* This asserts that the preceding pattern must be at the end of the string
* example: `world$` matches "world" only if it is at the end of a line or string.

### Quantifiers
These specifiy the number of occurances of a character or group of characters that the pattern should match with 

1. Asterisk (`*`)
* Matches 0 or more occurances of the preceding element
* example: `m*` matches "", "m", "mmm", etc. 

2. Plus (`+`)
* Matches 1 or more occurances of the preceding element
* example: `m+` matches "m", "mmm", etc. but not "".

1. Question Mark (`?`)
* Matches 0 or 1 occurances of the preceding element
* example: `m?` matches "" or "m"

1. Braces (`{n}`)
* Matches exactly `n` occurances of the preceding element
* example: `m{5}` matches "mmmmm"

### OR Operator
This allows you to match one pattern to another before or after the pipe symbol (`|`)
* example: `I ate a strawberry | apple | banana` matches "I ate a banana
* a more practical example is using the OR operator to validate e-mail addresses like this: 
`\b[A-Za-z0-9._%+-]+@(gmail\.com|yahoo\.com|outlook\.com)\b`

### Character Classes
One of the most important parts of regular expressions. These allow you to match a specific character type. Some examples include: 
* Dot (`.`) - x.z matches xyz, xwz, x4z, etc. 
* Bracket Expression (`[]`) - [xyz] matches x, y, or z but not any other character 
* Character Classes:
    * (`\d`) - matches any digit (0-9)
    * (`\D`) - matches any non digit characters like letters, punctuation, spaces, etc.
    * (`\w`) - matches any alphanumeric character, and underscore [`a-zA-Z0-9`]
    * (`\W`) - matches any non word character like numbers, punctuation, spaces, etc.
    * (`\s`) - matches any whitespace character (spaces, line breaks, tabs).
    * (`\S`) - matches any non-whitespace character. 

### Flags
Flags are used to modify regular expressions and change how pattern matching is performed. These are some of the most common of flags that are used:
* Case Sensitive (`i`) - makes the matchs case sensitive `/yourPatternHere/i`
* Golbal (`g`) - makes the expression search for all matches in the input, not stopping after the first match `/yourInputHere/g`
* Multiline (`m`) - change sthe behavior of `^` and `$` so they match the start and end of the line and not the whole string `/yourStringHere/m`
* Dotall (`s`) - allows the `.` character to match newline characters `/yourPatternHere/s`
* Sticky (`y`) - makes the expression start searching from the index indicated in the regex object's lastIndex property `/yourPatternHere/y`
* Unicode (`u`) - makes the expression assume individual characters as code points, ot code units, and thus match 32-bit characters as well `/yourPatternHere/u`

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
