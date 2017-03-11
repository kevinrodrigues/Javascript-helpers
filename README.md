# Pure Javascript helper functions

## Table of Contents

  1. [Flatten a simple Array](#array-flatten)
  1. [Remove all falsy values from Array](#array-filter-falsy-values)
  1. [Get last element in array](#array-return-last-array)
  1. [Get first element in array](#array-return-first-array)
  1. []()

## Arrays

  <a name="array-flatten"></a><a name="2.1"></a>
  - [1](#array-flatten)  **Flatten a simple array (1 Level deep)**.


    ```javascript
    // Flatten Array ES5
    var simpleArray = [['a', 'b', 'c'], [1, 2, 3], ['x', 'y', 'z']];

    simpleArray.reduce(function(a, b) {
      return a.concat(b); // ["a", "b", "c", 1, 2, 3, "x", "y", "z"]
    }, []);


    // Flatten Array ES6
    let simpleArray = [['a', 'b', 'c'], [1, 2, 3], ['x', 'y', 'z']];

    simpleArray.reduce((a, b) => a.concat(b), []); // ["a", "b", "c", 1, 2, 3, "x", "y", "z"]

    ```

  <a name="array-filter-falsy-values"></a><a name="2.1"></a>
  - [2](#array-filter-falsy-values) **Remove all falsy values**.


    ```javascript
    // Flatten Array ES5
    var simpleFalsyArray = ['a', '', 'c', undefined, null, 0];

    simpleFalsyArray.filter(function(value) {
      return !!value; // ["a", "c"]
    });


    // Flatten Array ES6
    let simpleFalsyArray = ['a', '', 'c', undefined, null, 0];

    simpleFalsyArray.filter((value) => !!value); // ["a", "c"]

    ```

  <a name="array-return-last-array"></a><a name="2.1"></a>
  - [3](#array-return-last-array) **Get last element in array**.


    ```javascript
    // Get last array element (assumes array exists).
    var simpleLastArray = ['foo', 'baz', 'fizz'];

    simpleLastArray[simpleLastArray.length - 1]; // fizz

    ```

  <a name="array-return-first-array"></a><a name="2.1"></a>
  - [4](#array-return-first-array) **Get last element in array**.


    ```javascript
    // Get first array element (assumes array exists).
    var simpleLastArray = ['foo', 'baz', 'fizz'];

    simpleLastArray[0]; // foo

    ```