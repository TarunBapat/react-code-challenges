- The Context API is a feature in React that allows you to share state or data across components without having to pass props manually through each level of the component tree. It provides a way to create a central store of data that can be accessed by any component within its scope.

- The Context API consists of two main components: the Context Provider and the Context Consumer.

- The Context Provider is responsible for defining the data or state that will be shared. It wraps around a group of components and provides them with access to the shared data. It acts as the source of truth for the data and allows components to subscribe to updates.

- The Context Consumer is used within components that need to access the shared data. It allows these components to subscribe to the data provided by the Context Provider and use it within their rendering logic.

- Here are the basic steps to use the Context API in React:

- Create a new context using the createContext function from React.
  Define a Context Provider component that wraps around the components that need access to the shared data. This component should render the Context.Provider component and provide the value prop with the data or state that you want to share.
  Use the Context Consumer component within the components that need access to the shared data. This component should render the Context.Consumer component and provide a function as its child. This function will receive the shared data as its argument and can be used within the component's rendering logic.
  Wrap your top-level component or components with the Context Provider to make the shared data available to the components within its scope.
  By using the Context API, you can avoid prop drilling (passing props through multiple levels of components) and easily share state or data between components that are not directly related in the component hierarchy. It provides a clean and efficient way to manage shared data in your React applications.

- https://codesandbox.io/s/peaceful-austin-8y2q6h
