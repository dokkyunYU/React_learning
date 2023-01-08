# key는 prop으로 그냥 접근할 수 없다.

key 그리고 ref는 특별한 값으로 취급되므로 설령 props에 포함되어 전달된다고 해도

```javascript
const Something = ({className, key, ...restProps}) =>
  React.createElement(
    'h1',
    {className, key},
    ...restProps
  )

React.createElement(Something, {className : 'myClass', key:'myKey'}, 'child1', 'child2')
```

위와 같이 구조분해할당을 하려고 하면 key가 empty로 반환된다고 경고를 보낸다.

key값을 접근하고 싶다면 props에 다른 key값을 설정해서(ex. myKey:'someKey') 보내는 식으로 간접참조할 수 있다.