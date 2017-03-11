# Pure Javascript helper functions

## Table of Contents

  1. [Arrays](#arrays)
  1. [Flatten a simple Array](#array-flatten)
  1. [Remove all falsy values from Array](#array-filter-falsy-values)

## Arrays

  <a name="array-flatten"></a><a name="2.1"></a>
  - [1.1](#array-flatten)  **Flatten a simple array (1 Level deep)**.


    ```javascript
    // Flatten Array ES5
    var simpleArray = [['a', 'b', 'c'], [1, 2, 3], ['x', 'y', 'z']];

    simpleArray.reduce(function(a, b) {
      return a.concat(b); // ["a", "b", "c", 1, 2, 3, "x", "y", "z"]
    }, []);


    // Flatten Array ES6
    var simpleArray = [['a', 'b', 'c'], [1, 2, 3], ['x', 'y', 'z']];

    simpleArray.reduce((a, b) => a.concat(b), []); // ["a", "b", "c", 1, 2, 3, "x", "y", "z"]

    ```

  <a name="array-filter-falsy-values"></a><a name="2.1"></a>
  - [1.2](#array-filter-falsy-values) **Remove all falsy values**.


    ```javascript
    // Flatten Array ES5
    var simpleFalsyArray = ['a', '', 'c', undefined, null, 0];

    simpleFalsyArray.filter(function(value) {
      return !!value; // ["a", "c"]
    });


    // Flatten Array ES6
    var simpleFalsyArray = ['a', '', 'c', undefined, null, 0];

    simpleFalsyArray.filter((value) => !!value); // ["a", "c"]

    ```