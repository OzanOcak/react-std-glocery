## react

yarn add react-icons

- the obj array stored in the useState , object can't be map, it alsi simulate fetching data.

local storage is used

```javascript
localStorage.setItem("shoppinglist", JSON.stringify(listItems));
```

#### prop drilling :

is a method to pass parameters/props to child components

#### control component :

means components can be control by user via inputs, which are beacically always recieve inputs

instead of array, we fetch data from local storage

```javascript
const [items, setItems] = useState(
  JSON.parse(localStorage.getItem("shoppinglist"))
);
```

#### useRef()

```javascript
const inputRef = useRef();
<input ref={inputRef}/>
<button onClick={()=>{inputRef.current.focus()}}/>
```
