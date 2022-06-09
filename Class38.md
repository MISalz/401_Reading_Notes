# Class38 Reading Notes

Reading

[React - Conditional Rendering](https://reactjs.org/docs/conditional-rendering.html)

In React, you can create distinct components that encapsulate behavior you need. Then, you can render only some of them, depending on the state of your application.

[React - Lists & Keys](https://reactjs.org/docs/lists-and-keys.html)

Rendering Multiple Components
You can build collections of elements and include them in JSX using curly braces {}.

Basic List Component
Usually you would render lists inside a component.

Extracting Components with Keys
Keys only make sense in the context of the surrounding array.

Keys Must Only Be Unique Among Siblings
Keys used within arrays should be unique among their siblings. However, they don’t need to be globally unique. We can use the same keys when we produce two different arrays:



[React - Forms](https://reactjs.org/docs/forms.html)

Controlled Components
In HTML, form elements such as \<input>, \<textarea>, and \<select> typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().

We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.

The textarea Tag
In React, a \<textarea> uses a value attribute instead. This way, a form using a \<textarea> can be written very similarly to a form that uses a single-line input.


The select Tag
React, instead of using this selected attribute, uses a value attribute on the root select tag. This is more convenient in a controlled component because you only need to update it in one place

The file input Tag
it is an uncontrolled component in React. It is discussed together with other uncontrolled components later in the documentation.

Handling Multiple Inputs
When you need to handle multiple controlled input elements, you can add a name attribute to each element and let the handler function choose what to do based on the value of event.target.name.

[React - Lifting State](https://reactjs.org/docs/lifting-state-up.html)

[React - Composition vs Inheritance](https://reactjs.org/docs/composition-vs-inheritance.html)

[Thinking in React](https://reactjs.org/docs/thinking-in-react.html)


Videos

Optional: [Hero Icons](https://www.youtube.com/watch?v=cVa1UiKPJN8)

Bookmark and Review

[React - Comprehensive Guide](https://tylermcginnis.com/reactjs-tutorial-a-comprehensive-guide-to-building-apps-with-react/)

[Heroicons](https://heroicons.com/)

----

## Things I want to know more about

----
[Home](https://github.com/MISalz/401_Reading_Notes/blob/main/README.md)