# Pure Javascript helper functions

## Table of Contents

  1. [Arrays](#arrays)

## Arrays

  <a name="array-flatten"></a><a name="2.1"></a>
  - [1.1](#array-flatten)  **Flatten a simple array (1 Level deep)**.


    ```javascript
    // Flatten Array ES5
    var simpleArray = [['a', 'b', 'c'], [1, 2, 3], ['x', 'y', 'z']];

    simpleArray.reduce(function(a, b) {
      return a.concat(b);
    }, []);


    // Flatten Array ES6
    var simpleArray = [['a', 'b', 'c'], [1, 2, 3], ['x', 'y', 'z']];

    simpleArray.reduce((a, b) => a.concat(b), []);

    ```

  <a name="array-filter-falsy-values"></a><a name="2.1"></a>
  - [1.2](#array-filter-falsy-values) **Remove all falsy values**.


    ```javascript
    // Flatten Array ES5
    var simpleFalsyArray = ['a', '', 'c', undefined, null, 0];

    simpleFalsyArray.filter(function(value) {
      return !!value;
    });


    // Flatten Array ES6
    var simpleFalsyArray = ['a', '', 'c', undefined, null, 0];

    simpleFalsyArray.filter((value) => !!value);

    ```