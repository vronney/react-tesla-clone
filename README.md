# React Tesla Clone App

## Telsa Clone App built to demonstate skills with ReactJS

```
npx create-react-app <name of folder> --template redux
```
**--template redux** used to add redux store.js to file

## Tools
* [ReactJS](https://reactjs.org/)
* [Redux](https://react-redux.js.org/)
* [Styled Components](https://styled-components.com/)
* [React Reveal](https://www.react-reveal.com/)
* [Netlify](https://app.netlify.com/) - used for hosting

## React useState
```
const [burgerStatus, setBurgerStatus] = useState(false)
```
Returns a stateful value, and a function to update it.

During the initial render, the returned state (<mark>state</mark>) is the same as the value passed as the first argument (<mark>initialState</mark>).

The setState function is used to update the state. It accepts a new state value and enqueues a re-render of the component.

```
setBurgerStatus(newState)
```
Used to show side menu

## Styled Components
```
npm install --save styled-components
```
`styled-components` utilises tagged template literals to style your components.

It removes the mapping between components and styles. This means that when you're defining your styles, you're actually creating a normal React component, that has your styles attached to it.

```
// Create a Title component that'll render an <h1> tag with some styles
const Title = styled.h1`
  font-size: 1.5em;
  text-align: center;
  color: palevioletred;
`;

// Create a Wrapper component that'll render a <section> tag with some styles
const Wrapper = styled.section`
  padding: 4em;
  background: papayawhip;
`;

// Use Title and Wrapper like any other React component – except they're styled!
render(
  <Wrapper>
    <Title>
      Hello World!
    </Title>
  </Wrapper>
);
```

## React Reveal

[React Reveal](https://www.react-reveal.com/) is an animation framework for React. It's MIT licensed, has a tiny footprint and written specifically for React in ES6. It can be used to create various cool reveal on scroll animations in your application. 

```
npm install react-reveal --save
```

Import effects from React Reveal to your project. Lets try Zoom effect first:

```
import Zoom from 'react-reveal/Zoom';
```

Place the following code somewhere in your render method:

```
<Zoom>
  <p>Markup that will be revealed on scroll</p>
</Zoom>
```

You should see zooming animation that reveals text inside the tag. You can change this text to any JSX you want. If you place this code further down the page you'll see that it'd appear as you scroll down.