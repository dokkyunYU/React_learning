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