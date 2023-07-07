# UnderstandingState

Notes on Stateful components

//for react `import {state} from 'react';`

-function body that defines the componet begins with the function call

`const [ counter, setCounter ] = useState(0)`

^adds state to the component>renders it initialized with the value of zero. `=useState(0)`

The function returns an array -two values -assign them to counter and setCounter using destructuring assignment.

``setTimeout( () => setCounter(counter + 1), 1000 )`

A function called setTimeout -passed it two parameters

1. a function to increment the counter state. `() => setCounter(counter + 1)` when this state modifying function is called, React re-renders the component. -the function body of the component function gets re-executed.

2. a timeout of one second
