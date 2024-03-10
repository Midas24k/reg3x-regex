# Title (replace with your title)

What is a Regular Expression or Regex as it commonly known. Regex are components that are building blocks that are used to define patterns for matching strings within text. So in short the cool algorithms you see on the spy movies that the hero uses to decipher and crack codes to save the day. While that is one thing that Regex can be used for in code, its not the only thing. Regex can be used to create complex search patterns for finding patterns, replacing, or manipulating text efficiently. The code that can be built with Regex can range from extremely simple to "what are you talking about" hard. Understanding the concepts of Regex is definitely allows for a powerful tool to be placed in the arsenal.

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.
In the example provided below using Regex and CSS through code you can highlight keywords and strings for higher visibility. This code require to Regular expressions in order to function properly, and the are as followed "keywordPattern" and "stringPattern". While this may seem like a simple thing used with a little creativity it can become complexed very quickly.

<script>
// Define keywords and their corresponding CSS classes
var keywords = ['function', 'var'];

// Regular expression pattern to match keywords
var keywordPattern = new RegExp('\\b(' + keywords.join('|') + ')\\b', 'g');

// Regular expression pattern to match strings
var stringPattern = /(["'])(?:(?=(\\?))\2.)*?\1/g;

// Get the code element
var codeElement = document.getElementById('code');

// Get the code content
var codeContent = codeElement.innerHTML;

// Highlight keywords
codeContent = codeContent.replace(keywordPattern, '<span class="keyword">$1</span>');

// Highlight strings
codeContent = codeContent.replace(stringPattern, '<span class="string">$&</span>');

// Update the code element with highlighted content
codeElement.innerHTML = codeContent;
</script>

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

- `stringPattern`

### Quantifiers

- `keywordPattern`

- `stringPattern`


### Grouping Constructs

- `keywordPattern`

- `stringPattern`


### Bracket Expressions

- `keywordPattern`

- `stringPattern`


### Character Classes

- `keywordPattern`

- `stringPattern`


### The OR Operator

- `keywordPattern`

- `stringPattern`

### Flags

- `keywordPattern`

- `stringPattern`


### Character Escapes

- `keywordPattern`

- `stringPattern`


## Author
Roderick Hughey
A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
