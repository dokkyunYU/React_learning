# reduce

```javascript
list.reduce((이어나가는 값, 리스트의 각 값들) => 원하는 리턴 값, 초기값)

// ex

mylist = ['1', '2', '3']
mylist.reduce((allstring, num) => allstring + num, '')

// 결과 : 123
```

# map

```javascript
list.map((리스트의 각 값들) => 원하는 리턴 값)

// ex

mylist = ['1', '2', '3']
mylist.map((num) => `<li>${num}</li>`)

// 결과 : [<li>1</li>, <li>2</li>, <li>3</li>]

```

# forEach

```js
list.forEach((value, index, array) => {})

//ex

mylist = [1,2,3,4,5];
mylist.forEach((value, index, array) => {
  console.log(value, index, array);
})
// 1, 0, [1,2,3,4,5]
// 2, 1, [1,2,3,4,5]
// 3, 2, [1,2,3,4,5]
// 4, 3, [1,2,3,4,5]
// 5, 4, [1,2,3,4,5]
```