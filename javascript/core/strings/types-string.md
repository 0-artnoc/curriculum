---
author: alexjmackey
type: normal
category: must-know
---

# Types - String


---

## Content

The primary way to declare a string value in JavaScript is to use quotes. Using single or double works the same:

```plain-text
let company1 = "Enki";
let company2 = 'Enki';
```

You can connect, usually called "concat", two strings together with the '+' operator:

```plain-text
let longText = "abc" + "def" + "ghi";
// longText is equal to "abcdefghi"
```

You can also use the backslash character to continue writing text on multiple lines:

```plain-text
var longerText = "abc\
def\
ghi";
```

There are also special characters that can be used by preceding the character with a backslash. Here are some common ones:

```plain-text
\’ single quote
\" double quote
\\ backslash
\n new line
\r character return
\t tab
```


---

## Practice

What special character is used to add a `new line` to strings denoted with quotes?

```javascript
let myString = 'this will ???
       be displayed on two lines';
```

- `\n`
- `+`
- `"`
- `\`
- `\r`
- `\t`


---

## Revision

Which one of the following is correct?

```plain-text
let company1 = "Enki";
let company2 = 'Enki';
```

???

- both
- first
- second
- none
