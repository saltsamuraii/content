🛠 Так как `filter` возвращает массив, то у полученного массива мы можем продолжать по цепочке вызывать другие методы массива.

```js
const nums = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

const result = nums.filter(num => num >= 5).map(...).reduce(...)
```

🛠 В `filter` в качестве функции можно передать конструктор `Boolean` . Таким образом можно легко и быстро отфильтровать все элементы, которые при приведении к boolean будут равны `false`.

```js
const num = 3

const elements = [0, "", "one", "two", num === 3 && "three", null].filter(
  Boolean
) // ['one', 'two', 'three']
```