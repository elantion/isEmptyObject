# typeOf
Check a object is empty

### Reference
http://stackoverflow.com/questions/4994201/is-object-empty

### Example
```js
isEmpty(""), // true
isEmpty(33), // true (arguably could be a TypeError)
isEmpty([]), // true
isEmpty({}), // true
isEmpty({length: 0, custom_property: []}), // true

isEmpty("Hello"), // false
isEmpty([1,2,3]), // false
isEmpty({test: 1}), // false
isEmpty({length: 3, custom_property: [1,2,3]}) // false
```