# Pure Javascript helper functions

## Table of Contents

  1. [Arrays](#arrays)

## Arrays

  <a name="array-flatten"></a><a name="2.1"></a>
  - [1.1](#array-flatten) Flatten a simple array, (1 Level deep)


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