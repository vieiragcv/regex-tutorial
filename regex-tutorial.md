# Title

Regex Tutorial by Gui Vieira

Applying logic to your code

## Summary

Also known as a "regular expression" is a sequence of characters that specifies a search pattern in a text. 

Basics Concepts to help you better navigate this tutorial:


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

What are Anchors?

Anchors are characters that does not match any specific character, but assert something about the string or the matching process. 


Beginning Anchor: "^"

  Determines the "location" for the beginning of a string or line 

  Example: Testing if the string "Florida" starts with the letter "F"

  const str = 'Florida';
  console.log(/^F/.test(str));

  Output: true




End Anchor "$"

  Determines the "location" for the end of a string or line

  Example: Testing if the string "Florida" ends with the letter "j"

  const str = 'Florida';
  console.log(/$j/.test(str));

  Outputs: false


### Quantifiers & Alternation

Plus "+"

  Matches 1 or more of the preceding token.

Star "*"

  Matches 0 or more of the preceding token.

Quantifier "{ x, x } { x, }"

  Matches the specified quantity of the previous token. {1,3} will match 1 to 3. {3} will match exactly 3. {3,} will match 3 or more.

Optional "?"

  Matches 0 or 1 of the preceding token, effectively making it optional.

Lazy "?"

  Makes the preceding quantifier lazy, causing it to match as few characters as possible. By default, quantifiers are greedy, and will match as many characters as possible.

Alternation " | "

  Acts like a boolean OR. Matches the expression before or after the | .
  It can operate within a group, or on a whole expression. The patterns will be tested in order.

### OR Operator



### Character Classes

Character Set

Negated Set

Range

Dot

Match Any

Word

Not Word

Digit

Whitespace

Not Whitespace

Unicode category

Not unicode category

Unicode script

Not unicode script

### Escaped Characters

Reserved characters "\+"

Octal escape "\000"

Hexadecimal escape "\xFF"

Unicode escape "\uFFFF"

Extended unicode escape "\u{FFFF}"

Control character escape "\cI"

Tab "\t"

Line feed "\n"

Vertical tab "\v"

Form feed "\f"

Carriage return "\r"

Null "\0"

### Flags

Ignore Case

Global Search

Multiline

Unicode

Sticky

Dotall

### Grouping and Capturing

Capturing Group (ABC)

Named capturing group

Numeric Reference

Non-Capturing Group

### Bracket Expressions



### Greedy and Lazy Match



### Boundaries

Word Boundary "\b"

  Matches a word boundary position between a word character and non-word character or position (start / end of string). See the word character class (w) for more info.

Not Word Boundary "/B"

  Matches any position that is not a word boundary. This matches a position, not a character.

### Back-references



### Look-ahead and Look-behind

Positive Look-ahead (?=ABC)
Negative Look-ahead (?!=ABC)

Positive Look-behind (?<=ABC)
Negative Look-behind (?<!ABC)

## Author

(replace with your information and a link to your profile)
