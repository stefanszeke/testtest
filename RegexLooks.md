
### Lookahead: `\w+(?=\t)` matches a word followed by a tab
### Negative lookahead: `\d+(?!\.)` matches a sequence of digits not followed by a period.

</br>

### Lookbehind: `(?<=\$)\d+` matches a sequence of digits preceded by a dollar sign
### Negative lookbehind: `(?<!19)\d{2}` matches a two-digit number that is not preceded by "19".

</br>

In regular expressions, "lookahead" and "lookbehind" are zero-width assertions, meaning they do not consume any characters in the input string as part of the match.

Lookahead:
A positive lookahead (?=...) asserts that the preceding pattern must be followed by the pattern inside the parentheses, but the pattern inside the parentheses is not included in the match.
For example,  \w+(?=\t) matches a word followed by a tab, but the tab is not included in the match.

Negative lookahead:
A negative lookahead (?!...) asserts that the preceding pattern must not be followed by the pattern inside the parentheses.
For example, \d+(?!\.) matches a sequence of digits not followed by a period.

Lookbehind:
A positive lookbehind (?<=...) asserts that the pattern inside the parentheses must precede the pattern outside the parentheses, but the pattern inside the parentheses is not included in the match.
For example, (?<=\$)\d+ matches a sequence of digits preceded by a dollar sign, but the dollar sign is not included in the match.

Negative lookbehind:
A negative lookbehind (?<!...) asserts that the pattern inside the parentheses must not precede the pattern outside the parentheses.
For example, (?<!19)\d{2} matches a two-digit number that is not preceded by "19".

Note that lookbehind assertions are not supported in all regex implementations and their use may be limited by the maximum length of the pattern they can handle.

### other regex stuff:
    Matching specific characters:
    [abc] matches any character that is either a, b, or c.

    Grouping and alternation:
    (dog|cat) matches either "dog" or "cat".

    Matching digits:
    \d matches any digit, equivalent to [0-9].

    Matching whitespaces:
    \s matches any whitespace character, including spaces, tabs, and line breaks.

    Matching word boundaries:
    \b matches a word boundary, such as a space or the edge of the string.

    Matching repetitions:
    a{2,4} matches between 2 and 4 consecutive "a" characters.

    Matching optional items:
    colou?r matches either "color" or "colour".

    Matching the start and end of a line:
    ^A matches lines that start with an "A".
    A$ matches lines that end with an "A".5
