CSS-Less
=======


What is Less?
----------------
* CSS pre-processor
* Extends CSS to use features similar to a programming language	


Variables
-----------
INPUT:

		// Variables
		@link-color:        #428bca; // sea blue
		@link-color-hover:  darken(@link-color, 10%);
		@images:			"../images";
		
		// Usage
		a,
		.link {
		  color: @link-color;
		}
		a:hover {
		  color: @link-color-hover;
		}
		.widget {
		  color: #fff;
		  background: url("@{images}/bg.png") @link-color;
		}

OUTPUT:

		a,
		.link {
		  color: #428bca;
		}
		a:hover {
		  color: #3071a9;
		}
		.widget {
		  color: #fff;
		  background: url("../images/bg.png") #428bca;
		}
