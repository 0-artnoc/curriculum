---
author: Stefan-Stojanovic

levels:
  - beginner
  - basic
  
aspects:
  - introduction
  - new

type: normal

category: how to

---

# Aggregation With $dayOfYear, $week and $dayOfWeek

---
## Content

For the document used in aggregation, make sure to check the Previous Document[1] footnote.

### $dayOfYear

The `$dayOfYear` date operator is used to extract the exact day of the year the document was created on. The output goes from 1-366.

Example:
```js
db.pokedex.aggregate(
   [
     {$match: {"name": "Bulbasaur"}},
     {
       $project:
         {
           DayOfTheYear: { $dayOfYear: "$Date" },
           _id: 0
         }
     }
   ]
)
```

Output:
```js
{ 
  "DayOfTheYear" : 282 
}
```

### $week

The `$week` date operator is used to extract the exact week of the year the document was made on. The output goes from 1-53.

**Note:** The weeks start counting on Sunday(`1`) each year. If the year stars on any other day, those days belong in week `0` and week `1` starts from the first Sunday of that year.

Example:
```js
db.pokedex.aggregate(
   [
     {$match: {"name": "Bulbasaur"}},
     {
       $project:
         {
           WeekOfTheYear: { $week: "$Date" },
           _id: 0
         }
     }
   ]
)
```
Output:
```js
{ 
  "WeekOfTheYear" : 40 
}
```

### $dayOfWeek

The `$dayOfWeek` date operator is used to extract the exact day of the week the document was made on. The output goes from 1-7, 1 being Sunday and 7 being Saturday.

Example:
```js
db.pokedex.aggregate(
   [
     {$match: {"name": "Bulbasaur"}},
     {
       $project:
         {
           DayOfTheWeek: { $dayOfWeek: "$Date" },
           _id: 0
         }
     }
   ]
)
```
Output:
```js
{ 
  "DayOfTheWeek" : 4 
}
```

---
## Practice

Fill in the blanks:

The ??? operator is used to extract the exact day of the year the document was made on as a number between ???.

The ??? operator is used to extract the exact week the document was made and as a number between ???

The ??? operator is used to extract the exact day of the week the document was created on ???

* `$dayOfYear`
* `1-366`
* `$week`
* `0-53`
* `$dayOfWeek`
* `as a number between 1-7`
* `as a word Sunday-Saturday`
* `0-365`
* `1-54`



---
## Footnotes

[1:Previous Document]
Here is the document used in the previous insight:
```javascript
// document without the date
{ 
	"_id": ObjectId("5d9d8a6a0b24990f19398209"),
  "name": "Bulbasaur",
	"type": "Grass"
}
// Document with the date
{ 
	"_id": ObjectId("5d9d8a6a0b24990f19398209"),
  "name": "Bulbasaur",
	"type": "Grass",
  "Date": ISODate("2019-10-09T07:21:14Z")
}
```
