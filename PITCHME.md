---
marp: true
title: Web Development Orientation
theme: uncover
---

<!-- backgroundColor: #393D3F -->
<!-- color: #D7FFF1-->

<style>
  code, pre {
    background-color: #393D3F;
    color: #D7FFF1;
  }

  h1 {
    color: red;
  }
</style>

# Objective

Use JavaScript's `map` method to create a transformed data set.

---

# Introduction To Map

![w:500](https://stephenliddell.files.wordpress.com/2012/09/world-political-map.jpg)

(No, it's not that kind of map.)

---

### What Does Map Do?

It creates a new data set based on the transformation function you pass it. It might look something like this:

```javascript
const doubled = numbers.map(multiplyBy2);
const titles = sentences.map(changeToTitleCase);
const tweetAvatars = bioPhotos.map(reduceImageSize);
```

---

### We Now Have New Data Based On Our Old Data

* `doubled` is a new array of doubled numbers.
* `titles` is a new array of strings Where Every Word Starts With A Capital Letter
* `tweetAvatars` is a new array of smaller bio pictures.
* Crucially, our old-- hold on... this deserves its own slide!

---

### Not Mutative

Crucially, our old data remains.

We have our small avatars for tweets, but we haven't overwritten our big bio photos!

---

![w:500](https://upload.wikimedia.org/wikipedia/en/d/dd/Gnomes_plan.png)

But what were we passing in as arguments to `map` back there? How do I use `map`? How does it _work_?

---

# Part Two: Functions All The Way Down

---

### Passing Objects

We're used to passing in objects on which an action is done.

```javascript
const number2 = multiplyBy2(num);
const title = changeToTitleCase(sentence);
const tweetAvatar = reduceImageSize(bioPhoto)
```

Those functions take in one piece of data, transform it, and return the new data.

---

### Passing In Actions

But if we have a collection of data, like an array, it would be handy if we could tell a function:

"Here's a transformation, run this on every piece of data in the collection and give me back that transformed collection."

And that's `map`!

---

### I Think I Get It, But I Could Use An Emoji-Based Explanation

Well... 😁!

---
```javascript
const ingredients = ['🐔', '🐮', '🐠'];
const food = ingredients.map(cook);
food === ['🍗', '🍔', '🍣'];

const oldWorld = ['🐴', '🏰', '🚂'];
const newWorld = oldWorld.map(modernize);
newWorld === ['🚗', '🏙', '🚆'];
```
---

### You Tell Map HOW To Transform Each Piece Of Data

It takes care of the rest!

---

### How Do I Get This "Map"?

* The `map` method is part of JavaScript's Array prototype.
* Because it's on that "blueprint", we get it "for free" on every array!

---

### Code Along

Let's `map` some arrays together!

---

### Designing UI Through Text - 60 Hours 

![w:300](https://i.giphy.com/media/13FrpeVH09Zrb2/source.gif)

* Organizing Content through HTML and Markdown
* READMEs and Blogging
* CSS Styling Concepts
* Coding Logic L2

---

### Beginning JavaScript, Layout, and Responsiveness - 100 Hours

![w:300](https://i.stack.imgur.com/wHqUD.gif)

* Introduction to JavaScript and UI Manipulation
* Positioning and The Box Model
* Responsive Design with Media Queries, Flexbox, and Grid
* Coding Logic L3

---

### Advanced JavaScript - 100 Hours

![w:400](https://media.giphy.com/media/xT9IgzoKnwFNmISR8I/source.gif)
* Arrays, Objects, and Loops
* Callbacks and Higher Order Functions
* APIs and Asynchronous Programming
* Coding Logic L4