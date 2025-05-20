# JavaScript Cheatsheet: Object & Array Methods

A handy reference for core JavaScript object and array methods, with examples to quickly recall syntax during interviews or development.

---

## 🧩 Object Methods

### 1. `Object.keys()`

Returns an array of an object's keys.

```js
const obj = { a: 1, b: 2 };
console.log(Object.keys(obj)); // ["a", "b"]
```

### 2. `Object.values()`

Returns an array of an object's values.

```js
console.log(Object.values(obj)); // [1, 2]
```

### 3. `Object.entries()`

Returns an array of key-value pairs.

```js
console.log(Object.entries(obj)); // [["a", 1], ["b", 2]]
```

### 4. `Object.assign()`

Copies values from one or more objects to a target object.

```js
const target = { a: 1 };
const source = { b: 2 };
const result = Object.assign(target, source);
console.log(result); // { a: 1, b: 2 }
```

### 5. `hasOwnProperty()`

Checks if an object has a specific key.

```js
console.log(obj.hasOwnProperty("a")); // true
```

---

## 📚 Array Methods

### 1. `map()`

Creates a new array with results of calling a function on every element.

```js
const nums = [1, 2, 3];
const squared = nums.map(n => n * n);
console.log(squared); // [1, 4, 9]
```

### 2. `forEach()`

Executes a provided function once for each array element.

```js
nums.forEach(n => console.log(n));
```

### 3. `filter()`

Creates a new array with elements that pass a test.

```js
const even = nums.filter(n => n % 2 === 0);
console.log(even); // [2]
```

### 4. `reduce()`

Executes a reducer function on each element, returning a single output value.

```js
const sum = nums.reduce((total, n) => total + n, 0);
console.log(sum); // 6
```

### 5. `find()`

Returns the first element that passes a test.

```js
const found = nums.find(n => n > 1);
console.log(found); // 2
```

### 6. `includes()`

Checks if an array includes a value.

```js
console.log(nums.includes(2)); // true
```

### 7. `concat()`

Merges two or more arrays.

```js
const arr1 = [1, 2];
const arr2 = [3, 4];
const combined = arr1.concat(arr2);
console.log(combined); // [1, 2, 3, 4]
```

### 8. Spread Operator `...`

Expands or merges arrays/objects.

```js
const merged = [...arr1, ...arr2];
console.log(merged); // [1, 2, 3, 4]
```

### 9. `slice()`

Returns a shallow copy of a portion of an array.

```js
const sliced = nums.slice(1);
console.log(sliced); // [2, 3]
```

### 10. `splice()`

Changes the contents of an array (remove/replace/add).

```js
nums.splice(1, 1, 10); // Replaces index 1
console.log(nums); // [1, 10, 3]
```

---

Use this as a quick guide to review core concepts and syntax. Practice with small exercises to memorize!
