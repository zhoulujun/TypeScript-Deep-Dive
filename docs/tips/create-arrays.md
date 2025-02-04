## Creating arrays

Creating an empty array is super easy: 

```ts
const foo: string[] = [];
```

If you want an array to loop over: 

```ts
// what many people like
[...new Array(6)]; 
// or (what I like more)
Array.from({length: 6})
```

If you want to create an array pre-filled with some content use the ES6 `Array.prototype.fill`: 

```ts
const foo: string[] = new Array(3).fill('');
console.log(foo); // ['','',''];
```

If you want to create an array of a predefined length with calls you can use the spread operator: 

```ts
const someNumbers = [...new Array(3)].map((_,i) => i * 10);
console.log(someNumbers); // [0,10,20];
```
