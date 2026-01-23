# Manipulating Text and Streams

## Chapter 4 - Regular Expression Essentials
Regexes are special patters to identify and match text, eg. phone numbers and parameters.\n

How to create a regex, iteratively\n

1. Create a short list of valid terms.\n
2. Add some items to the list that look valid at a glance but aren't quite right, like an email without anything in front of the @.\n
3. Build a regex that matches a correct email address.\n
4. Refine the expression to eliminate the invalid addresses.\n
5. Repeat the privous step until most invalid addresses are eliminated.\n


regex syntax\n
.*      (.) means any character, followed by (\*) which means any number of times.\n
@       (@) the symbol @.\n

regex quantifiers.\n
regex marks that specify a size.\n

Quantifier  Meaning\n
*           any number of characters.\n
+           At least one character.\n
?           Between zero and one character.\n
{n}         Exactly *n* occurences of the character.\n
{n,}        *n* or more occurences of the character
{n,m}       Between *n* and *m* occurrences of the character.\n

Specifiers  Meaning\n
[A-Z]       Any full uppercase part of the alphabet.\n
[A-Za-z0-9] Any uppercase character or lowercase character or number.\n
metacharacters - ranges defined by a representative character.\n
.           Any character except for a line break.\n
\w          Any word (alphanumeric) character, including the underscore; shorthand for [a-zA-Z0-9].\n
\W          Any non-word character, which is anything not in \w set above.\n
\s          Any whitespace character (such as a space or tab).\n
\S          Any non-whitespace character.\n
\d          Any digit character [0-9].\n
\D          Any non-digit character.\n
[^]         Use before a character to exclude any characters following it from the regex.\n
^[]         This regex has to start the line. place regex expression inside [].\n
\           Escape a character.\n

Capture group - breka up expressions into smaller parts, only the small parts have to match.\n
Specifier   Meaning.\n
(.+)        Ignore at least one character in this place.

Use regex expressions 101 to test and break down regexes. URL: (https//.regex101.com).\n

## Getting to grips with grep.\n
