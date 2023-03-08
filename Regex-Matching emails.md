Regex- Matching Emails

Regular Expresssion (also know as Regex) is a series of characters that make a search pattern. Regex is a powerful tool that is used in different languages and allows developers to find or replace text in a program. 

## Summary
This gist will go over this pattern that matches an email.

    /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/


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
Anchors are used to ensure that matches are found at the start or end of the source string, or at the start of end for a line in multi-line text. Our example shows the "^" anchor being used at the beginning 

    ^: Indicates the start of a string or line.

    $: Indicates the end of a string or line.

Our example shows the "^" anchor being used at the beginning and the "$" anchor at the end of the pattern, indicating the start and end of out line.

### Quantifiers
Quantifiers declare quantities of data as part our patterns. In our example, we see the "+" quantifier used. This matches the pattern one or more times. Provided are some other quantifiers we might see in Regular Expression.

    *—Matches the pattern zero or more times

    +—Matches the pattern one or more times

    ?—Matches the pattern zero or one time

    {}—Curly brackets can provide three different ways to set limits for a match


### Grouping Constructs
Grouping allows us to treat expressions as a single unit. 

### Bracket Expressions
Bracket Expressions is also known as a character set. The brackets list the characters that may qualify for a mactch in our search. Referencing back to this portion of our pattern, 

    [a-z0-9_\.-]

the brackets have a set of characters in them. The characters within the brackets are what we are refrencing in our search. So in our example it is saying to match anything conatained within the brackets.


### Character Classes
Character classes allow for us to chooose characters based on their classification. There are two fundemental character classes:

- Word characters - Numbers and letters.
- Non-word characters - Spaces and punctuation marks.

Some examples of these characters are:
     
     . - Matches any single character except newline characters
     \s - Matches whitespace characters (space and tab)
     \S - Not whitespace 
     \w - A word character (numbers,letters and uderscores) 
     \W - Not work characters 
     
Going back to our example, we can see these character classes used within brackets, indicating what exactly we are matching. 

## Author
Rickie Flores is a full-stack developer student at the University of Washington  student at the University of Washington
