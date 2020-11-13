---
author: kapnobatai136

type: normal

category: must-know

tags:
  - introduction
  - insert

---

# INSERT

---

## Content

Adding new data into your table is as simple as writing `INSERT INTO table VALUES`.

Consider the following `fruits` table:

| id | name      |
|----|-----------|
| 1  | Raspberry |

To add a new fruit, you'd write:

```sql
INSERT INTO fruits VALUES
(2, 'Pineapple');
```

Now, return all the values[1] in the `fruits` table and you'll get:

| id | name      |
|----|-----------|
| 1  | Raspberry |
| 2  | Pineapple |


> 💡 This is a short introduction to the `INSERT` keyword. We'll explain how everything works in the next workout.

---

## Practice

Adding values to your table is done using the ??? keyword.

- INSERT
- SELECT
- FROM
- ADD

---

## Revision

Insert the following data into the `employees` table:

```sql
??? employees ???
(9, 'John', 'Developer')
```

- INSERT INTO
- employees
- VALUES
- INSERT
- FROM
- SELECT

---

## Footnotes

[1:Select All]
To return all the values in a table, you can use the `*` character:

```sql
SELECT * FROM fruits
```