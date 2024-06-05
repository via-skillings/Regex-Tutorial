# Regex-Tutorial

Regular expressions (regex) are powerful tools for pattern matching and search operations in strings. They offer a concise and flexible way to identify specific patterns within text. This tutorial covers the basics of regex syntax, common metacharacters, and practical examples for effective usage.

## Summary

In this tutorial, we'll explore a regex pattern for matching email addresses. The regex we'll discuss is:
```m
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```
We'll break down each component of this regex and explain how it matches email addresses effectively. Additionally, we'll provide practical examples of using this regex pattern in various programming languages for email validation.

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
Anchors are used to specify positions within the text. They include:
```m
^: Matches the start of a string.
$: Matches the end of a string.
\b: Matches a word boundary.
\B: Matches a non-word boundary.
```
For example, the regex "^cat" would match "cat" only if it appears at the beginning of a line, while "cat$" would match "cat" only if it appears at the end of a line.

### Quantifiers
Quantifiers specify the quantity of characters or groups to match. They include:
```m
*: Matches zero or more occurrences.
+: Matches one or more occurrences.
?: Matches zero or one occurrence.
{n}: Matches exactly n occurrences.
{n,}: Matches n or more occurrences.
{n,m}: Matches at least n and at most m occurrences.
```
For example, "ba+" would match "ba", "baa", "baaa", and so on.

### OR Operator
The OR operator "|" is used to match one of several possible patterns. For example, "cat|dog" would match either "cat" or "dog".

### Character Classes
Character classes define sets of characters to match. They include:
```m
[abc]: Matches any of the characters inside the brackets.
[^abc]: Matches any character not inside the brackets.
\d: Matches any digit (equivalent to [0-9]).
\w: Matches any word character (equivalent to [a-zA-Z0-9_]).
\s: Matches any whitespace character.
```
For example, "[aeiou]" would match any vowel.

### Flags
Flags modify regex behavior. Common flags include:
```m
i: Case-insensitive matching.
g: Global matching (matches all occurrences).
m: Multiline matching.
```
For example, the regex "/cat/g" with the "g" flag would match all occurrences of "cat" in a string.

### Grouping and Capturing
Parentheses are used for grouping and capturing parts of a regex pattern. For example, "(abc)+" would match "abc" one or more times and capture it as a group.

### Bracket Expressions
Bracket expressions match specific ranges of characters. For example, "[a-z]" matches any lowercase letter.

### Greedy and Lazy Match
Quantifiers are greedy by default, meaning they match as much as possible. Adding a "?" after a quantifier makes it lazy, matching as little as possible.

For example, ".*?" matches the smallest possible string.

### Boundaries
Boundaries specify positions in the text, such as word boundaries (\b) or non-word boundaries (\B).

For example, "\bcat\b" would match "cat" only if it appears as a whole word.

### Back-references
Back-references allow referring to previously matched groups. For example, "(cat) \1" matches "cat cat".

### Look-ahead and Look-behind
Look-ahead (?=) and look-behind (?<=) assertions match a pattern only if it is followed by or preceded by another pattern, respectively. For example, "cat(?=dog)" matches "cat" only if it is followed by "dog".

### Solution
**/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/** is the regex pattern johndoe_1@gmail.com

## Author

Made by [Olivia Skillings](https://github.com/via-skillings), a web development student with a love for all things prehistoric.