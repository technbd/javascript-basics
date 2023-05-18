### Variables

> Variables are like "labeled jars" for a value in JavaScript. We can store a value and give it a name, so that we can...
>
> - recall it
> - use it
> - or change it later on.

**Basic syntax**

```js
let someName = value;
let age = 55;
```

**Recall variables**

```js
let hens = 4;
let roosters = 2;
hens + roosters; // 6
```

**Update values**

```js
let hens = 4;
hens – 1 // 3
hens; // still 4
hens = hens -1;
hens // 3
```

**CONST**

> const works just like let, except you CANNOT change the value

```js
const hens = 4;
hens = 20; // error
const age = 17;
age = age + 1; //error
```

**Why use constant?**

> Once we cover Arrays & Objects, we'll see other situations where const makes sense over let.

```js
const pi = 3.14;
const daysInWeek = 7;
```

**VAR**

> Before let & const, var was the only way of declaring variables. These days, there isn't really a reason to use it.

```js
var x = 7.4;
```

**What is the value of eggCount?**

```js
let eggCount = 42;
eggCount + 2;
```

**What is the value of rating after this code runs?**

```js
const rating = 7.5;
rating = 8;
```

**What is the value of wind_speed?**

```js
let windSpeed = 76;
windSpeed += 5;
windSpeed--;
```

### Booleans

> Booleans are simple True or False values <br>
> Yes or No. 1 or 0.

```js
let isLoggedIn = true;
let gameOver = false;
const isWaterWet = true;
```

**Variable change type**

```js
let numDonuts = 13; // number
numDonuts = true; // Now Boolean
numDonuts = 12; // back to number
```

### Strings

> In JavaScript, Strings are pieces of text or strings of characters.
> <br>
> We wrap them in quotes

```js
let firstName = 'ziigy'; // single quotes work
let msg = "hello"; // double quotes work
let bad = " this '; // This DOES NOT work
```

**Stings are indexed**

> Each character has a corresponding index (a positional number)

```js
// String has length property
let firstName = "Ziggy";

// Access individual characters using index:
firstName.length; // 5
firstName[0]; // "z"
firstName[3]; // "g"

// Even though length is 5...
firstName[5]; // does not work
```

**String Methods**

> Strings come with a set of built-in methods, which are actions that can be performed on or with that particular string.
>
> We can do things like...
>
> - Searching within a string
> - Replacing parts of a string
> - Changing case (upper/lowercase)

**Changing case**

```js
let msg = "hello";
let yellMsg = msg.toUpperCase(); // HELLO

let angry = "Leave";
angry.toLowerCase(); // leave
```

**trim**

```js
let greeting = " leave ";
greeting.trim(); // 'leave'
```

**indexOf**

```js
let x = "catdog";
x.indexOf("cat"); // 0
x.indexOf("dog"); // 3
x.indexOf("z"); // -1
```

**slice**

```js
let str = "superabc";
str.slice(0, 5); // super
str.slice(5); // abc
```

**replace**

```js
let str = " hello gello haha";
str.replace("hello", "tello"); // tello gello haha;
```

**What is the value of age?**

```js
Const age = '5' + '5';
```

**What dose this evaluate to?**

```js
"pecan pie"[7];
```

**What dose this evaluate to?**

```js
"pup"[3];
```

**What is the value of song?**

```js
let song = "London calling";
song.toUpperCase();
```

**What is the output of cleanInput?**

```js
let userInput = " abcD ";
let cleanInput = userInput.trim().toLowerCase();
```

**What is the value of index?**

```js
let park = "yellostone";
const index = park.indexOf("stone");
```

**What is the value of index?**

```js
let yell = "go away!!";
let index = yell.indexOf("!");
```

**What does this evaluate to?**

```
'garbage!'.slice(2).replace('b', ' ');
```

**String escapers**

> - \n - newline
> - \' - single quote
> - \" - double quote
> - \\\ - backslash

**String template literals**

> Template literals are strings that allow embedded expressions, which will be evaluated and then turned into a resulting string.
> <br> > `WE USE BACK-TICKS NOT SINGLE QUOTES` > <br> > \`I am a template literal\` > <br> \* The back-tick key is usually above the tab key

```js
` I counted ${4 + 3}`; // I counted 7;

let user = "abc";
`welcome ${user}`; // welcome abc;

`gameOver ${user.toUpperCase()}`; // gameOver ABC;

let item = "cucumber";
let price = 6;
let quantity = 5;
`You  bought ${quantity} ${item}, total price: $${price * quantity}`; // You bought 5 cucumber, total price: $30;
```

### Null and Undefined

> - Null
>
>    <ul>
>        <li>"Intentional absence of any  value"</li>
>        <li>Must be assigned</li>
>    </ul>
>
> - Undefined
>
>    <ul>
>       <li>Variables that do not have an  assigned value are undefined</li>
>    </ul>

**null**

```js
let loggedInUser = null; // explicitly nothing
loggedInUser = "Alan"; // user login
```

**undefined**

```js
let pickles; // We didn't assign a value
pickles; // undefined
pickles = "are very gross";

// Undefined also comes up in others situations:
let food = "tacos";
food[7]; // undefined
```
