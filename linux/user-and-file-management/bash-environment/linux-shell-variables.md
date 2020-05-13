---
author: kapnobatai136

aspects:
  - introduction

type: normal

category: must-know

tags:
  - introduction
  - linux
  - variables

---

# Variables

---
## Content

Think of *variables* as a box. 

They are used to store information. To make them easily identifiable, you put a label on them. 

Let's try creating a variable now:

```bash
best_app="Enki"
```

> **Note:** don't add any spaces around the `=` sign or you'll get an error saying `"Command not found"`.

We've taken the `"Enki"` information, and stored it in our `best_app` box:

![variable-mental-model](https://img.enkipro.com/fa537341f3027f1cea7b76ecc3398e9d.png)

To print this variable, you'd type:

```bash
echo $best_app
Enki
```

> **Note:** when you are referencing variables, you need to prefix a `$` sign to the variable name. Otherwise, you are only printing the name of the variable.

```bash
echo best_app
best_app
```

---
## Practice

Create a variable named `good_dog` that stores `"Artemis"`, and then print it:

```bash
???="???"
echo ???
Artemis
```

* good_dog
* Artemis
* $good_dog
* $Artemis

---
## Revision

Which of these variable declarations will throw an error?

```bash
a="foobar"

b = foobar

c=foobar
```

???

* b
* a
* c
