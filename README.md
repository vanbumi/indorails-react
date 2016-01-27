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



