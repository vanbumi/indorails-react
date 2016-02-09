# IndoRails - React

## Hello World

    <!DOCTYPE html>
    <html>
    <head>
	    <meta charset="UTF-8" />
	    <title>Hello React!</title>
	    <script src="build/react.js"></script>
	    <script src="build/react-dom.js"></script>
	    <script src="https://cdnjs.cloudflare.com/ajax/libs/babel-core/5.8.23/browser.min.js"></script>
    </head>
    <body>
	    <div id="example"></div>
	    <script type="text/babel">
	      ReactDOM.render(
	        <h1>Hello, world!</h1>,
	        document.getElementById('example')
	      );
	    </script>
    </body>
    </html>

#### Separate File

Create helloword.js file.

    ReactDOM.render(
    	<h1>Hello, world!</h1>,
    	document.getElementById('example')
    ); 

    <script type="text/babel" src="src/helloworld.js"></script>

## Comments

	<!DOCTYPE html>
	<html>
	  <head>
	    <meta charset="utf-8" />
	    <title>React Tutorial</title>
	    <script src="https://cdnjs.cloudflare.com/ajax/libs/react/0.14.6/react.js"></script>
	    <script src="https://cdnjs.cloudflare.com/ajax/libs/react/0.14.6/react-dom.js"></script>
	    <script src="https://cdnjs.cloudflare.com/ajax/libs/babel-core/5.8.23/browser.min.js"></script>
	    <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/2.1.1/jquery.min.js"></script>
	    <script src="https://cdnjs.cloudflare.com/ajax/libs/marked/0.3.2/marked.min.js"></script>
	  </head>
	  <body>
	    <div id="content"></div>
	    <script type="text/babel" src="scripts/example.js"></script>
	    <script type="text/babel">
	      // To get started with this tutorial running your own code, simply remove
	      // the script tag loading scripts/example.js and start writing code here.
	    </script>
	  </body>
	</html>

### Component Structure:

	- CommentBox
  		- CommentList
    		- Comment
  		- CommentForm

### CoomentBox Component

	// tutorial1.js
	var CommentBox = React.createClass({

		render: function() {
			return (
					<div className="commentBox">
						Hello, world! This a CommentBox.
					</div>	
				);
		}	
	}); 
	ReactDom.render(
		<CommentBox />,
		document.getElementById('content')
	);

(to be continue ...)

# Tutorial Video	

## The Links
	<script src="https://cdnjs.cloudflare.com/ajax/libs/react/0.14.6/react.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/react/0.14.6/react-dom.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/babel-core/5.8.23/browser.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/2.1.1/jquery.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/marked/0.3.2/marked.min.js"></script>

## Create Component	

	<h1>Bucky - Component</h1>

	<div id="content"></div>

	<script type="text/babel">
		var BuckysComponent = React.createClass({
			render: function() {
				return(
						<h2>My Name is Dyo</h2>
					);
			}
		});
		ReactDOM.render(
			<BuckysComponent />,
			document.getElementById("content")
		);
	</script>

## Create Multiple Component

	<h2>Multiple Element</h2>

	<div id="content2"></div>

	<script type="text/babel" >
		var DyoComponent = React.createClass({
			render: function() {
				return(
					<h3>My Name is Brandon</h3>
				);
			}
		});
		ReactDOM.render(
			<div>
				< DyoComponent />
				< DyoComponent />
				< DyoComponent />
				< DyoComponent />
			</div>,	
			document.getElementById('content2')
		);
	</script>

## How to use property

	<h2>Multiple Element and how to use properties and attributs</h2>

	<div id="content2"></div>

	<script type="text/babel" >
		var DyoComponent = React.createClass({
			render: function() {
				return(
					<h3>My Name is {this.props.user} and I like to eat {this.props.food} </h3>
				);
			}
		});
		ReactDOM.render(
			<div>
				< DyoComponent user="Brandon" food="Steak" />
				< DyoComponent user="Ersya" food="Sushi" />
				< DyoComponent user="Dyo" food="Pasta" />
				< DyoComponent user="Nancy" food="Burger" />
			</div>,	
			document.getElementById('content2')
		);
	</script>

## Children

	<h1>Children</h1>

	<div id="content"></div>

	<script type="text/babel">

		var DyosComponent = React.createClass({
			render: function() {
				return(
					# always under div tag
					<div>	
						<h3>{this.props.user}</h3>
						<p>{this.props.children}</p>
					</div>	
				);
			}
		});
		ReactDOM.render(
			# create closed tab
			# always under div tag
			<div>
				< DyosComponent user="DyoMedio" >How do you get my name?</DyosComponent> 
				< DyosComponent user="Brandon" >He is an awesome kid</DyosComponent>
			</div>,
			document.getElementById('content'));
		
	</script>

My another React in my CodeJournal [link!](https://github.com/vanbumi/CodeJournal/blob/master/react/getting-start.md)

