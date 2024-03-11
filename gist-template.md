# What is a Regex

What is a Regular Expression or "Regex" as it commonly known. Regex are components that are building blocks that are used to define patterns for matching strings within text. So in short the cool algorithms you see on the spy movies that the hero uses to decipher and crack codes to save the day. While that is one thing that Regex can be used for in code, its not the only thing. Regex can be used to create complex search patterns for finding patterns, replacing, or manipulating text efficiently. The code that can be built with Regex can range from extremely simple to "what are you talking about" hard. Understanding the concepts of Regex is definitely allows for a powerful tool to be placed in the arsenal.

## Summary

In the example provided below using Regex and CSS through code you can highlight keywords and strings for higher visibility. This code require to Regular expressions in order to function properly, and the are as followed `keywordPattern` and `stringPattern`. While this may seem like a simple thing used with a little creativity it can become complexed very quickly.

![alt text](<Regular Expression snippet.png>)

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

For those who are new to Regex. The characters used to create different effects are known as "Regex Component". Below I have a compiled some common knowledge about Regex Components that will help with the understanding of how the code above works by breaking down all of the components.

Literals: These are characters that match themselves. For example, the regex a will match the letter "a".

Meta-characters: These are special characters with reserved meanings in regex. Some common meta-characters include:

- . (dot): Matches any single character except newline.
- ^ (caret): Matches the start of a string.
- $ (dollar): Matches the end of a string.
- *: Matches the preceding element zero or more times.
- +: Matches the preceding element one or more times.
- ?: Matches the preceding element zero or one time.
- | (pipe): Acts as an OR operator.
- () (parentheses): Groups parts of the pattern together.
- [] (square brackets): Defines a character class.
- {} (curly braces): Specifies the number of occurrences of the preceding element.
- \ (backslash): Escapes meta-characters or introduces special sequences.

Character Classes: These allow you to match specific sets of characters. For example, [abc] will match any of the characters 'a', 'b', or 'c'.

Quantifiers: These specify how many times a character or group should occur. For example, *, +, ?, and {} are quantifiers.

Anchors: Anchors are used to specify the position of the match within the text. ^ and $ are examples of anchors.

Groups and Capturing: Parentheses ( ) are used to create groups, and they can also be used for capturing matched text.

Escapes: The backslash \ is used to escape special characters, allowing you to match them literally.

Modifiers: Modifiers are used to change the behavior of the regex pattern. For example, i for case-insensitive matching, g for global matching, etc.

These components can be combined in various ways to create complex patterns for text matching and manipulation. Understanding how to use these components effectively is essential for working with regex.

### Anchors

- `keywordPattern`
`\\b`: This is a word boundary anchor. It matches a position where a word character (alphanumeric or underscore) is not followed or preceded by another word character. It helps to ensure that the matched keyword is a whole word and not part of a longer word.

### Backreference
- `stringPattern`
`\`:  This backreference, matches the same text as most recently matched by the 1st capturing group (["']). It ensures that the closing quote matches the same type as the opening quote. 

### Quantifiers

- `stringPattern`
`*?`: This quantifier matches between zero and unlimited times, as few times as possible (non-greedy). It allows the pattern to match the shortest possible string that satisfies the regex.


### Grouping Constructs

- `keywordPattern`
`( )`: These parentheses define a capturing group. In this context, they group the keywords together, allowing us to match any of them as a single entity.

- `stringPattern`
`(?:(?=(\\?))\2.)*?`: This is a non-capturing group. It allows us to group parts of the pattern without capturing the matched text.


### Bracket Expressions

- `stringPattern`
`(["'])`: This part of the pattern matches either a single or double quote. It uses a character class ["'] which matches any single character inside the brackets, in this case, either a single quote ' or a double quote ".


### Delimiter

- `keywordPattern`
`keywords.join('|')` :This part joins the keywords array into a single string with '|' (pipe) as the delimiter. This effectively creates a regex alternation, allowing the pattern to match any of the keywords.

### Flags

- `keywordPattern`
`'g'`:This is a flag that stands for "global". It indicates that the regular expression should search for all matches within the input string, rather than stopping after the first match.

- `stringPattern`
`/g` : This flag indicates a global search, which means it searches for all matches rather than stopping after the first match.


### Character Escapes

- `stringPattern`
`(?=(\\?))`: This is a positive lookahead assertion (?=) which ensures that the following pattern is matched, but does not consume any characters. Here, it looks for an optional backslash \\? (escaped because \ is a special character in regex), which is captured in a capturing group (\\?). This part allows us to handle escaped quotes.


## Author

Roderick Hughey
A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
