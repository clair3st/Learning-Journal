### React 
## Overview
*Resources:* 
[Lecture](https://www.youtube.com/watch?v=FRjlF74_EZk)
[Docs](https://react.dev/learn)

# What is React?
A js library. Agnostic user interface library. It's used to create interfaces (charts, bars, websites, applications)
ReactDom used for webpages. React library doesn't have to be used in web browser, always needs a companion library like ReactDom or React360, or for server. React isn't a framework (unlike angular, which is more robust), allows it to be tailored to many different scenarios.

# What is the dataflow of React?
Data flows down one way. Reduces breakpoints of applications with data. Flows 'down' through the app/document tree

# How do we make a React element a DOM element?
Until it passes through react dom

# React is a User Interface ______.
Library

# Which direction does data flow in React?
one way, one of the first frameworks to introduce and becoming most common

# Every component manages its own ____.
State, this is what gets passes to children components


## Components
*Resource:* [Tutorialspoint](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)

# What is a component?
A function or class. Contain all the required methods and properties to allow for an independent and modular part of the application. Different functions that control different components of the use interface
Basic structure:
```
import React from 'react';

class Something extends React.Component {
  render() {
    return(
       <section>
         <h1>Header for Something</h1>
         <p>Text that is all about Something.<p>
       </section>
    )
  }
}

export default Something
```
# What are the characteristics of a component?
- Reusable
- Replaceable
- Modualar
- portable
- extensible
- encapsualted - keeps internal workings seperated
- independent

# What are the advantages of using component-based architecture?
 - Faster and easier developement due to reusability of components.
 - easier deployments as can sqap things out without impacting entire system
 - Increased reliabilty by using componenets already in use.
 - Reduced cost due to ease of using thrid party components
 - independent - can be developed at the same time


## Props
*Resource:* [Free Code Camp](https://www.freecodecamp.org/news/how-to-use-props-in-reactjs/)

# What is “props” short for?
Properties, like properties of an object

# How are props used in React?
Used to pass data between components. It's passed into a component, similar to how attributes are used in HTML.
```
<ComponentName property1="value" property2="value" property3="value" />
```

# What is the flow of props?
React only allows the follow of data from parent component to child. This means child can't pass data back to parent, or edit the data received from parent.
