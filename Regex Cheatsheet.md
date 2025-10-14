## Description 

Regex (regular Expression) is a special string pattern used to search, match or manipulate text. 

It can match letters, numbers, spaces or even complex patterns like e-mails or URLS. 

Used in: 
- Validation
checks if input fits a format: e-mail addresses, phone numbers, postal codes, passwords

- Searching
Find specific pattern in a text: All dates in a document, words starting with capital letter, hashtags in a tweet.

- Extraction
Pull out pieces of text: Extract numbers from a string, URLS from a webpage, words between quotes

- Replacement/Cleaning
Change or remove text that fits a pattern: Remove extra spaces, censor bad words, reformat dates

- Splitting text in advanced ways

## Basics
| Symbol | Meaning | Example |
|--------|---------|---------|
| `.`    | Any character except newline | `a.b` matches `acb`, `a1b` |
| `\d`   | Digit (0-9) | `\d\d` matches `12`, `45` |
| `\D`   | Non-digit | `\D` matches `a`, `!` |
| `\w`   | Word character (letter, digit, underscore) | `\w+` matches `Hello_123` |
| `\W`   | Non-word character | `\W+` matches `!@#` |
| `\s`   | Whitespace (space, tab, newline) | `\s+` matches `"  "` |
| `\S`   | Non-whitespace | `\S+` matches `"word"` |
| `*`    | 0 or more | `a*` matches `""`, `"a"`, `"aa"` |
| `+`    | 1 or more | `a+` matches `"a"`, `"aaa"` |
| `?`    | 0 or 1 | `a?` matches `""` or `"a"` |
| `{n}`  | Exactly n | `a{3}` matches `"aaa"` |
| `{n,}` | n or more | `a{2,}` matches `"aa"`, `"aaa"` |
| `{n,m}`| Between n and m | `a{2,4}` matches `"aa"`, `"aaa"`, `"aaaa"` |
| `^`    | Start of string | `^Hello` matches `"Hello world"` |
| `$`    | End of string | `world$` matches `"Hello world"` |
| `[abc]`| a, b, or c | matches `"a"` in `"cat"` |
| `[^abc]`| not a, b, or c | matches `"d"` in `"dog"` |
| `[a-z]`| range a to z | matches `"f"` |
| `[0-9]`| any digit | matches `"7"` |
| `(abc)`| Group | `(ab)+` matches `"ab"`, `"abab"` |
| `vertical bar`    | OR | `cat|dog` matches `"cat"` or `"dog"` |

## Quantifiers
| Symbol  | Meaning         | Example                                     |
|---------|----------------|--------------------------------------------|
| `*`     | 0 or more       | `a*` matches `""`, `"a"`, `"aa"`          |
| `+`     | 1 or more       | `a+` matches `"a"`, `"aaa"`               |
| `?`     | 0 or 1          | `a?` matches `""` or `"a"`                |
| `{n}`   | Exactly n       | `a{3}` matches `"aaa"`                     |
| `{n,}`  | n or more       | `a{2,}` matches `"aa"`, `"aaa"`           |
| `{n,m}` | Between n and m | `a{2,4}` matches `"aa"`, `"aaa"`, `"aaaa"`|

## Anchors
| Symbol | Meaning         | Example                           |
|--------|----------------|----------------------------------|
| `^`    | Start of string | `^Hello` matches `"Hello world"` |
| `$`    | End of string   | `world$` matches `"Hello world"` |

## Character sets
| Symbol   | Meaning        | Example                   |
|----------|----------------|---------------------------|
| `[abc]`  | a, b, or c     | matches `"a"` in `"cat"` |
| `[^abc]` | not a, b, or c | matches `"d"` in `"dog"` |
| `[a-z]`  | range a to z   | matches `"f"`            |
| `[0-9]`  | any digit      | matches `"7"`            |

## Group Alternation 

| Symbol  | Meaning | Example                          |      |                             |
| ------- | ------- | -------------------------------- | ---- | --------------------------- |
| `(abc)` | Group   | `(ab)+` matches `"ab"`, `"abab"` |      |                             |
| `       | `       | OR                               | `cat | dog`matches`"cat"`or`"dog"` |





