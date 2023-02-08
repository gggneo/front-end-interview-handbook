---
title: Front end utility functions
slug: coding/utility-function
sidebar_label: Utility functions
---

These are the front-end version of LeetCode questions, but with less emphasis on complicated algorithms and more focused on practical use cases. However, they could also be questions simply being the same LeetCode problem but you are required to answer in JavaScript.

Almost all existing utility functions you will be asked exist within the JavaScript language or famous third-party libraries like Lodash/Underscore, with the most famous being `debounce` and `throttle`. However, Lodash's implementation is extremely over-engineered - reusing a lot of abstract functions and supporting weird and obscure use cases for older browsers and you're not expected to produce such level of complexity in an interview.

## Basic examples

- `debounce()`/`throttle()`
- `cloneDeep()`
- `groupBy()`
- `chunk()`/`map()` with follow up of `mapAsync`(`Promise.all`) then `mapWithChunksAsync`
- Convert all keys within an object into snake_case/camelCase
- `document.querySelectorAll` (limited to just tags selectors)
- [Observer pattern](https://addyosmani.com/resources/essentialjsdesignpatterns/book/#observerpatternjavascript)

The best way to prepare is to get your hands dirty by implementing them yourself and writing test cases for them. Because you're writing functions, pay attention to the time complexity as well. Don't write a function that runs in O(n<sup>2</sup>) if it can pretty easily be written in O(n).

Candidates are expected to take just around 10-15 minutes for a basic question. If you can tell that you received a basic question, try to finish within the suggested duration and do not intentionally take the entire interview to do one question. In most cases, you are expected to answer another small coding question.

## Advanced examples

Advanced questions are usually given to more senior candidates and expect around 25-30 minutes to complete or arrive at a minimally working solution.

- Write a templating engine that does variables substitution and simple conditionals
- Implement `JSON.stringify()`
- Generate table of contents/outline from a HTML page (similar to Google Docs autogenerated outline)

## Tips

- Always try to write pure functions
- If you're writing a recursive function, ask whether there's a maximum stack depth limit
- Some nested data structures can have recursive references to itself. Do clarify that there are no self-references/cycles within the object/ask if you need to handle them (usually the answer is No)