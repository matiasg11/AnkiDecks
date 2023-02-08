# React Anki Deck

### 01 - What is React and how is it constructed?

#### React is a JavaScript library for building fast and interactive user interfaces. The operations in React are components, which are essentially a piece of user interface. When we are building applications with React, we are building a bunch of independent, isolated and reusable components, combining them to build complex user interfaces. Every React app has at least one component, which we refer to as the root component. This component represents the entire application and contains other child components. 
For example, for Twitter, the page can be split into navbar, profile, trends and feeds. Then the feeds have individual tweet coomponents and the functionality to like or retweet them.

### 02 - What is a component?

#### In terms of implementation, a component is typically implemented as a JavaScript class that has some state and a render method.
![Alt text]( "Component Class")

#### The state is the data that we want to display when the component is rendered, and the render method is responsible for describing what the UI should look like.

#### The output of this render method is a react element, which is a simple plain JavaScript object that reacts to a DOM element. It's not a real DOM element, it's just a plain JavaScript object that represents the DOM element in memory.

#### React keeps a lightweight representation of the DOM in memory which we refer to as the virtual DOM. Unlike the browser or the real DOM, this virtual DOM is cheap to create. When we change the state of a component, we get a new react element. React will then compare this element and it's children with the previous one, it figures out what has changed, and then it will update a part of the real DOM to keep it in sync with the virtual DOM.

#### With React, unlike vanilla JavaScript and query, we no longer have to work with the DOM API in browsers. In other words, we no longer have to write code in query or manipulate the DOM, or attach event handlers to DOM elements. You simply change the state of our components and React will automatically update the DOM to match that state. And that's exactly why this library is called React, because when the state changes, React essentially reacts to the state change and updates the DOM.
