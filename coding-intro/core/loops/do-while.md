---
author: kapnobatai136

type: normal

category: must-know

---

# DO..WHILE

---
## Content

In a `DO..WHILE` loop, you start by running the code the first time, followed by checking a condition. If that evaluates to `true`, you run the code again.

Going back to our sandwiches, let's say you want to make sure there is always one sandwich available.

```plain-text
hungry = true
sandwiches_made = 0

DO
  Make a sandwich.
  Increase sandwiches_made by 1.
WHILE (
  hungry AND 
  sandwiches_made <= 3
)
```

Now, you'll make the sandwich, and later decide if more sandwiches are required (based on your condition).

---
## Practice

In a `DO..WHILE` loop, which happens first?

???

* The code is ran.
* The condition is checked.