Regex Tutorial

Regular Expressions are patterns that match a combination of characters in a string.
JavaScript supports regular expressions mostly for text search and text replacement.
You can also find and replace a character or sequence of characters within a string.
They are also frequently used to validate input. This regex matches character information for valid e-mail addresses.

Summary

What is JavaScript RegExs? 

A JavaScript RegEx is a sequence of characters that forms a search pattern. 
You can define what needs to be searched in a text with the help of regular expressions.
These expressions can be of any number of characters, be it alphabets, digits or special characters. 
They are more commonly used for text search and text replacement operations.
This is the regex code that we will be anaylizing today is: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/


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
The anchors used to contain this regular expression are: ^ to start, and $ to finish.

### Quantifiers
Quantifiers define the number of occurrences of a string.
The most commonly used quantifiers are ‘+’, ‘*’ and ‘?’. 

 + - Indicates one or more occurrence of the character n 

 * - Indicates zero or more occurrences of the character n 

 ? - Indicates zero or one occurrence of the character n 

### Grouping Constructs
There are three groups being captured in this example. Group #1 is the username of the e-mail account [a-z0-9_\.-].
The second group captures the domain name or e-mail service being used [\da-z\.-]. 
Lastly, the third group captures the domain extention (i.e .com or .net) [a-z\.]{2,6}

### Bracket Expressions
Much like the groups in this example, there are also 3 bracket expressions. 
The information in the bracket expressions is opened and closed between brackets like this []. 
This indentifies which information is allowed to be matched.

Bracket Expression #1: [a-z0-9_\.-] - includes case sensitive characters from a-z, numbers from 0-9 an underscore, periods and hyphens.

Bracket Expression #2: [\da-z\.-] - includes all digits, case sensitive characters from a-z, periods and hyphens

Bracket Expression #3: [a-z\.] - includes case sensitive characters from a-z and periods.

### Character Classes
A character class. Matches any one of the enclosed characters. You can specify a range of characters by using a hyphen,
but if the hyphen appears as the first or last character enclosed in the square brackets, 
it is taken as a literal hyphen to be included in the character class as a normal character.

### OR operator
The logical OR ( || ) (logical disjunction) operator for a set of operands is true if and only if one or more of its operands is true. 
It is typically used with boolean (logical) values. When it is, it returns a Boolean value

### Flags
A flag variable, in its simplest form, is a variable you define to have one value until some condition is true, 
in which case you change the variable's value. It is a variable you can use to control the flow of a function or statement, 
allowing you to check for certain conditions while your function progresses.

### Character Escapes
The \ is known as the escape code, which restore the original literal meaning of the following character. 
Similarly, * , + , ? (occurrence indicators), ^ , $ (position anchors) have special meaning in regex.
You need to use an escape code to match with these characters.

## Author

Melina Morales 
