
  <p>I've spent the past 3 weeks learning React.<br>
  I find that doing theory and practical tests help me to improve my understanding of how React works.</p>

  <p>I've been using the following resources simultaneously to improve my understanding:
    <ul>
      <li><a href="https://www.codecademy.com/" target="_blank">Codecademy Learn ReactJS: Part 1</a></li>
      <li><a href="https://www.freecodecamp.org/" target="_blank">Free Code Camp React section</a></li>
      <li><a href="http://www.reactbites.com/" target="_blank">React Bites</a></li>
      <li<a href="https://reactforbeginners.com/" target="_blank">React for beginners by Wes Bos </a></li>
    </ul>
  </p>
  <h2>This is what I've learnt so far with Codeacademy:</h2>

  <p>React is a JavaScript library used for building user interfaces.</p>

  <p>You can create an event listener by giving a JSX element a special attribute.<p>
  <img onClick = {myFunc} />

  <p>Event listeners attribute name should be like onClick, onMouseOver etc.<br>
  The word <em>on</em> plus <em>type of event</em> you're listening for.<br>
  An event listener attributes value = Function<br>
  The example above would only work if myFunc was a valid function.
  </p>

  <p>In JSX event listener names are written in camelCase.</p>

  <a href="https://codepen.io/SundeepToor/pen/JBYgRv" target="_blank">onClick event image swap</a>

  You cannot inject an if statement into a JSX expression because of how JSX is compiled.

  JSX conditions - If statements that work.

  <a href="https://codepen.io/SundeepToor/pen/MBaNRQ" target="_blank">JSX Conditions</a>

  <a href="https://codepen.io/SundeepToor/pen/pZgzRV" target="_blank">JSX Conditionals: &&</a>

  If you want to create a list of JSX elements, then <em>.map()</em>

  <a href="https://codepen.io/SundeepToor/pen/EpPYbB" target="_blank">.map in JSX </a>

  <p>Sometimes the list will need keys. A key is a JSX attribute that needs to be unique.
  React uses them to keep track of lists.<br>
  If you don't use keys when you need to, React might accidentally scramble list items in wrong order!</p>

  <p>A list needs keys if:
  <ul>
  <li>list-items have memory from one render to the next (e.g. When to-do list renders, each item must remember whether it was checked off) </li>
  OR
  <li>A list's order might be shuffled (e.g. A list of search results might be shuffled from one render to the next)</li>
  </ul>
  </p>
  <a href="https://codepen.io/SundeepToor/pen/jpWNRQ" target="_blank">How to get <em>.map()</em> to produce a unique key each time it loops.</a>

  <p>React.createElement - write React code without JSX!<br>
  JSX EXPRESSION<br>
  const h1 = <h1>Hello World</h1>;<br>
  CAN BE WRITTEN AS:<br>
  const h1 = React.createElement(<br>
  "h1",<br>
  null,<br>
  "Hello, world"<br>
  );</p>

  <p>Components are reusable code that usually render html.</p>

  <p><em>import React from 'react';</em><br>
  This line creates a new variable, it's value is a particular imported JavaScript object.</p>

  <p>Every component must come from a <u>component class</u>.</p>

  <p>Use <em>component class</em> to produce as many components as you want. To make a component 
  class use <em>React.Component</em></p>

  <p><em>React.Component</em> is a JavaScript class to create your own component class:<br>
  <em>class</em> YourComponentNameGoesHere <em>extends React.Component { }</em><br>
  Component class variable names must begin with capital letters.</p>

  <p>The <em>render()</em> method should contain a return statement. Usually the return statement returns  a JSX expression.
  Whenever you make a component, that component inherits all of the methods of its component class.</p>

  <p><a href="https://codepen.io/SundeepToor/pen/xJZgjq">React Component Class</a></p>

  <p>A multiline JSX expression expression should always be wrapped in parentheses <em>()</em></p>

  <p><a href="https://codepen.io/SundeepToor/pen/VBePEQ">Use a variable attribute in a component</a></p>

  <p>You can put calculations that need to be performed before a component renders within the <em>render()</em> function.</p>

  <p><a href="https://codepen.io/SundeepToor/pen/ejJvPy">Logic in a render function</a></p>

  <p><a href="">Display an item from an array of objects</a></p>
  
  <p><a href="https://codepen.io/SundeepToor/pen/OwMpYN">When using a conditional in a render function, the if statement appears before the return.</a></p>

  <p><a href="https://codepen.io/SundeepToor/pen/OwMpKN">Using <em>this</em> in a component.</a></p>

  <p>Render functions contain event listeners.<br>
  <a href="https://codepen.io/SundeepToor/pen/ejJWmK">Using an event listener in a component.</a></p>

  <p>In React, you define event handlers as methods on a component class.</p>


