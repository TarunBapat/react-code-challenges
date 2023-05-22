- React.memo is a higher-order component (HOC) in React that is used to optimize the performance of functional components by preventing unnecessary re-renders. It's similar to React.PureComponent for class components.

- When a component is wrapped with React.memo, it will only re-render if its props have changed. If the component receives the same props, React.memo will return the previously rendered result, avoiding the need to re-render the component and its children.

- https://codesandbox.io/s/dank-https-g3b5eu
