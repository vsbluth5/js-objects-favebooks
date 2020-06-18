# Favorite Books - JSON Edition!

### The goal

This lab is housed in the `objects.js` file. 

In this lab, you'll start to deal with JSON objects that organize data more and more clearly. We'll start with an array of favorite books, but each book is keyed to a person's name.

For example, to print Zara's favorite book, you'd use the code `console.log(favorite_books["zara"])`.

Open up the console to see the output.

### Tips, examples, & answers

Iteration for an object is really similar to iteration for a list, with just one extra step. Here's an example:

```js

let treatments = {
  "sunburn": "apply some aloe vera",
  "dehydration": "drink some water",
  "headache": "drink some water and consider taking a pain-reliever"
}

// First collect the issues in an array:
let issues = Object.keys(treatments)
// At this point, issues should be the array ["sunburn", "dehydration", "headache"]

// Then, iterate as normal:
issues.forEach(issue => {
  console.log(`If you have ${issue}, you should ${treatments[issue]}`)
})
```

If you need a boost, you can see answers to challenge 1 and challenge 3a.

<details>
  <summary> Click to see a solution to challenge 1 </summary>

  ```js

    // Reassign values for a key in a dictionary the same way we replace items in a list:
    favorite_books["jeff"] = "The Martian"
    // You can print it out to check whether it works by also including this line of debugging code:
    console.log(favorite_books["jeff"])

  ```

</details>
<br>

<details>
  <summary> Click to see a solution to challenge 3a </summary>

  ```js
  let people = Object.keys(favorite_books) // This should collect JUST the keys and return them as an array.
  ```

</details>
<br>
