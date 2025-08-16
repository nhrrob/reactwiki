##  1. React Basics


<br/>Last Modified: Aug 14, 2025 <br/>
<br/>Date: Aug 14, 2025 <br/>

Note: *For sample code follow repository mentioned below (at the end)* <br>


### Steps
# React Learn — Minimal Cheatsheet

#### 1 - Components
- Functions that return JSX.
- Must start with a **Capital letter**.

```jsx
function MyButton() {
  return <button>Click</button>;
}
```

#### 2 - JSX
- HTML-like syntax inside JavaScript.
- Allows embedding expressions with `{}`.

```jsx
const name = "React";
<h1>Hello {name}</h1>;
```

#### 3 - Props
- Pass data from parent → child.
- Read-only values.

```jsx
function Welcome({ user }) {
  return <h1>Hello {user}</h1>;
}
<Welcome user="Robin" />;
```

#### 4 - State
- For dynamic, interactive values.
- Managed with `useState`.

```jsx
import { useState } from "react";
const [count, setCount] = useState(0);
```

#### 5 - Events
- Event handlers are camelCase.
- Pass function, not string.

```jsx
<button onClick={() => setCount(count + 1)}>+</button>
```

#### 6 - Lists & Keys
- Render lists with `.map`.
- `key` must be unique & stable.

```jsx
{items.map(item => <li key={item.id}>{item.name}</li>)}
```

#### 7 - Conditional Rendering
- Use ternary, `&&`, or `if`.

```jsx
{isLoggedIn ? <Dashboard /> : <Login />}
```

#### 8 - Lifting State Up
- Share state by moving it to the closest common parent.

#### 9 - Hooks
- **useState**: state management.  
- **useEffect**: side effects (fetch, subscriptions).  
- **useContext**: share data globally.  

```jsx
useEffect(() => {
  document.title = `Count: ${count}`;
}, [count]);
```

#### 10 - Thinking in React (Process)
1. Break UI into components.  
2. Build static version.  
3. Identify minimal state.  
4. Identify state owner.  
5. Add inverse data flow.  
6. Add interactivity.  


<br>


### We are done!

- Congratulations! You have successfully covered React Basics. <br>


### Note
- TBA
<br>

### Bonus:
- TBA

<br>


### <a href='https://github.com/nhrrob/reactwiki'>Back to React Wiki</a>
