# Scripting Lesson 10 Demo Starter

Run local development using the following:

```
npm install
npm start
```

## Instructions

Use what you've learned about loops to solve the problem challenges.

First we'll work with `for` for some basic practice.

1. Create a loop that prints every number between 1 and 50 to the console.
2. Create a loop that prints every even number between 3 and 25 to the console. 

Now practice working with array loops. First, add the following array declaration to your script:

```js
 var items = [
    "chicken",
    "eggs",
    "milk",
    "salt",
    "sriracha sauce"
  ];
```  

Let's try using `for` loops with this pattern:

```js
for (var i=0; i < __array__.length; i++) {
    var item = __array__[i];
    // ... other code as needed goes here
}
```

3. Display each value stored in `items` individually to the console.
4. Populate a list of items into the shopping list on the page based on the values stored in `items`.

Now let's try using `.each()`.

5. Try to duplicate the same idea as above using a `.each()` instead of `for`. 

Once you've got it working you can remove the `for` loop in favor of the `.each()` loop.

Let's try something more involved. Lets set up our application here to allow the user to add a new item to the shopping list. There is an array of existing items, `items` and we only want to add a new item to it if its not already on the list. 

6. Create an event handler that responds when `#add-item-form` is submitted.
7. Inside, prevent the default action.
8. Store the current value of the `#new-item` field in a variable, `newItem`.
9. Declare a variable `matchFound` and set it to `false`. 
10. Next, use a loop to compare the new value to each individual item stored in `items`. If an item matches, set `matchFound` to `true`.  
11. Finally, if a match was found after the loop ends, send this message to the feedback box:

    ```html
    That item is already on the list.
    ```

    Otherwise, use `items.push(newItem)` to add it to the list and then send this message to the feedback box:

    ```html
    [newItem] was added to the list
    ```