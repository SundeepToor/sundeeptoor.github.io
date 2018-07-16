<div class="blog">
	<h3>Getting Component to interact</h3>
	
	<p>Render methods can also return another kind of JSX - <em><a href="https://codepen.io/SundeepToor/pen/gjPxZb" target="_blank">component instances</a></em></p>
	<h3>Exporting Components<h3>
	<p><em>export const nameOfItem = {};</em></p>
	<p>You can make multiple exports within the same file</p>
	<p>In a different file, <em>import</em> the name of the variable from the first file</p>
	<p>e.g. In NavBar.js: <em>export class NavBar extends React.Component . . .</em><br>
	In ProfilePage.js: <em>import {NavBar} from './NavBar.js';</em>
	</p>
	
	<h3><em>this.props</em> - Store dynamic information in React</h3>
	<p>A component can pass information to another component</p>
	<p>Every component has something called <em>props</em><p>
	<p><em>props</em> is an object that holds information about component.</p>
	<p>To see a component's props object, use expression <em>this.props</em></p>
	<p>Give component an attribute to pass info to<br>
	<em><MyComponent foo = "bar" /></em><p>

	<p>To pass information to a component, you need a <em>name</em> for the information that you want to pass</p>
	<p>If you want to pass info that isn't a string, wrap info in curly braces</p>

	<p>How you would pass an array:<br>
	<em><Greeting myInfo = { [ "top", "secret", "12"] } /></em><br>	<Greeting name="Henry" city="London" age={2} /></p>

	<p>Passing information to a component's <em>props</em> object</p>
	<p><em>ReactDOM.render(<Greeting firstName = 'Roberta'/>, document.getElementById('app'));</em></p>

	<h3><a href="https://codepen.io/SundeepToor/pen/WKrXEP" target="_blank">How to make a component display passed-in info</a></h3>
	<ol>
		<li>Find the component class that is going to recieve that info</li>
		<li>Include <em>this.props.name-of-info</em> in that components class's render method's return statement</li>
	</ol>

	<p><a href="https://codepen.io/SundeepToor/pen/djGZZz" target="_blank">Pass props from component to component</a></p>
	
	<p>You can use <em>props</em> to make decisions</p>
	<p>You can check if a particular value has been given to a prop before returning another prop</p>
	<p>You often pass functions as props.<br>
	It is common to pass event handler functions.
</p>

	<p>You have to define an event handler before you can pass one anywhere</p>
	<p>You define an event handler as a method on the component class, just like the <em>render</em> method.</p>

	<p><a href="https://codepen.io/SundeepToor/pen/VBeyXg" target="_target">Using props to make decision</a><p>

	<p><a href="https://codepen.io/SundeepToor/pen/RBrxBz" target="_blank">Recieve an event handler as a prop</a></p>
 	
	<h3>Naming Convention</h3>
	<p>First name you choose -> Event handler</p>
	<p>Second name you choose -> name of prop you pass to</p>

	<p>What type of event handler are you listening for?<br>
	e.g. <em>click</em>, you name event handler <em>handleClick</em></p>

	<p>Your prop name should be the word <em>on</em> plus your event type. e.g. <em>onClick</em></p>

	<h3><em>this.props.children</em></h3>
	<p>Every component's <em>props</em> object hs a property named <em>children</em>
	<p><em>this.props.children</em> will return evrthing in between a component's opening and closing JSX tags.</p>

	<p>Components don't have to be self closing!</p>
	<p><em><MyComponentClass></em><br>
	this.props.children would return everything in here<br>
	<em></MyComponent></em></p>

	<p>e.g. <em><BigButton><br>
	<em>I am a child of BigButton</em><-- this.props.children would equal this text<br>
	<em></BigButton></em></p>

	<p><em><BigButton /></em><-- this.props.children would equal undefined</p>
	
	<p><em><BigButton></em><br>
	<em><LittleButton /></em><-- this.props.children would equal <LittleButton />
	<em></BigButton></em></p>

	<p>If a component has more than one child between JSX tags, <em>this.props.children</em> will return children in an array.</p>

	<p>If a component has only one child <em>this.props.children</em> will return single child, not wrapped in an array.</p>

	<p><em>if(this.props.children instanceof Array){<br>
		titleText += 's' ;<br>
		}</em><-- checks if this.props.children returns an array(multiple items), then adds an 's' to the title to make it plural.</p>

	<h3>defaultProps</h3>
	<p><em><button</em><em>></em><br>
		{this.props.text}<br>
	<em></button</em><em>></em></p>

	<p>If nobody passes any <em>text</em> to <em>button</em>, then it will display blank.</p>
	<p>It would be better if <em>button</em> could display default message instead.</p>

	<p><a href="https://codepen.io/SundeepToor/pen/wxGWay" target="_blank">Giving a component class a property named <em>defaultProps</em></a></p>

</div>
