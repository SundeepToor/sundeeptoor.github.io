<div class="blog">
	<h3><em>this.state</em></h3>
	<p>Setting initial state</p>
	<p>React component can access dynamic info in 2 ways: <em>props</em> and <em>state</em></p>

	<p>To make component have <em>state</em>, give the component a <em>state</em> property.</p>

	<p>Property should be declared inside of a constructor method:<br>
	<em>constructor (props){<br>
	super(props);<br>
	this.state={mood: 'decent'};<br>
	}</em></p>

	<p><em>this.state</em> should equal an object. Object represents the initial "state" of any component instance.</p>

	<p><em>constructor</em> and <em>super</em> are both features of ES6.</p>

	<p>React components <u>always</u> have to call <em>super</em> in their constructors to be set up properly.</p>

	<p>Methods should <u>never</u> be comma-separated!</p>

	<h3><a href="https://codepen.io/SundeepToor/pen/djMOoL" target="_blank">Access a component's state</a></h3>
	
	<p>To <u>read</u> a component's <em>state</em>, use the expression<br>
	<em>this.state.name-of-property</em></p>

	<p>Just like <em>this.props</em>, you can use <em>this.setState</em> from any property defined inside of a component class's body.</p>

	<h3>Update <em>state</em> with <em>this.setstate</em></h3>

	<p><em>this.setState( )</em> takes two arguments</p>
	<ul>
		<li>An object will update the component's state</li>
		<li>A callback (rarely need this)</li>
	</ul>

	<p><em>this.setState()</em> takes an object, and merges that object with the component's current state.</p>

	<p>If there are properties in the current state that aren't part of that object, then those properties remain how they were.</p>

	<p><a href="https://codepen.io/SundeepToor/pen/pZywgQ" target="_blank">Call <em>this.setState</em> from another Function</a></p>

	<p>The most common way to call <em>this.setState()</em> is to call a custom function that wraps a <em>this.setState()</em> call.</p>

	<p>
	<ol>
		<li>A user triggers an event (click event), triggered by clicking on a <button></li>
		<li>The event from Step 1 is being listened for (e.g. <em>onClick</em> attribute)</li>
		<li>When listened-for event occurs, it calls an <em>event handler</em> function ()</li>
		<li>Inside of the body of the <em>event handler</em>, <em>this.setState()</em> is called</li>
		<li>The component's <em>state</em> is changed</li>
	</ol>
	</p>
	<p><a href="https://codepen.io/SundeepToor/pen/zLqbWx" target="_blank">Setting state with this.setState</a></p>

	<p>Whenever you define an event handler that uses <em>this</em>, you need to add <em>this.methodName = this.methodName.bind(this)</em> to your constructor function.</p>


	<p><a href="https://codepen.io/SundeepToor/pen/EpKXWa" target="_blank">Example: Change color</a></p>

	<p>Any time that you call <em>this.setState()</em>, <em>this.setState()</em> automatically calls <em>.render()</em> as soon as the state has changed.</p>

	<p>This is why you can't call <em>this.setState()</em> from inside <em>.render()</em>. An infinite loop would be created!</p>





</div>
