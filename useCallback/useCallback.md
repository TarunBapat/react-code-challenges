- In this example, we have a MyComponent that renders a count value and two buttons. Clicking the "Increment" button increments the count, and clicking the "Decrement" button decrements the count.

- We define the increment and decrement functions using the useCallback hook. Each function is memoized and will only be recreated if their dependencies change.

- Since the increment and decrement functions don't have any dependencies in this example, they will remain the same throughout the component's lifecycle unless the component is unmounted and remounted.

- By using useCallback for the increment and decrement functions, we ensure that the functions are memoized and their references remain the same. This prevents unnecessary re-renders of child components that rely on these callbacks.

- Using useCallback in this example optimizes the performance of MyComponent by avoiding unnecessary re-creation of the increment and decrement functions on each render, resulting in a more efficient and performant React application.

- https://codesandbox.io/s/dank-https-g3b5eu
