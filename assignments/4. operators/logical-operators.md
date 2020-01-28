# Logical Operator

1. 🥇What's the output of the following, write the output next to the code as comment.

* [ ] Logical AND operation

```js
true  && true; // true
true  && false; // false
false && true; // false
false && false; // false
"foo" && "bar"; // "bar"
"bar" && "foo"; // "foo"
"foo" && ""; // ""
""    && "foo"; // ""
" "   && "John" && "" && false // ""
false && "Hey" && undefined // false
"undefined" && false && 42 // false
```

* [ ] Logical OR operationHello World" > "Super Mario
```js
true  || true; // true
true  || false; // true
false || true; // true
false || false; // false
"foo" || "bar"; // "foo"
"bar" || "foo"; // "bar"
"foo" || ""; // "foo"
""    || "foo"; // "foo"
" "   || "John" || "" || false // " "
false || "Hey" || undefined // "Hey"
"undefined" || false || 42 // "undefined"
```

2. 🥈You have two variables i.e `isGuestOneVeg` and  `isGuestTwoVeg` according to the value using logical && and || opeartor do the following.

* [ ] If both are veg "Only offer up vegan dishes."
* [ ] At least one veg  "Make sure to offer up some vegan options."
* [ ] Else, "Offer up anything on the menu"
```js
let isGuestOneVeg = false;
let isGuestTwoVeg = false;
// Your code goes here

if(isGuestOneVeg && isGuestTwoVeg)
{
    alert("Only offer up vegan dishes.");
}
else if(isGuestOneVeg || isGuestTwoVeg)
{
    alert("Make sure to offer up some vegan options.");
}

else {
    alert("Offer up anything on the menu");
}
```


3. 🎖Using the variable `temperature` and logical operators do the following
* [ ] If temperature is less then 32 alert "It is freezing outside"
* [ ] If the temperature is greater then 110 alert "It is hot outside"
* [ ] else 'Go for it. It is pretty nice out'
```js
let temperature = 4;
// Your code goes here
let a = (32 > temperature ? "It is freezing outside":null) || (110 < temperature ? "It is hot outside":null) || "Go for it. It is pretty nice out";

alert(a);

```

4. 🎖 Output of this and the reason behind the output.
```js
alert( alert(1) || 2 || alert(3) );

Answer: 
It will show modal window twice, for 1 and 2. 
Because alert always returns undefined. 

[eg.

let a = (alert(1)); 
console.log(a) // undefined ]

So if we replace inner alerts with undefined 
the expression will look like this -

alert(undefined || 2 || undefined);

As we know that logical OR always searches for first true value so it will iterate untill it gets the first truthy value that is 2. Thats why the first inner alert will also be executed.
```