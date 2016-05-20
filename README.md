#CSS Editor.
With this application you can edit CSS files using functions and variables.
Currently the editor is in the beta stage so its not ready for production use but you may
use it and offer any feedbacks. 

The purpose of this application is to offer a way to pre-process sass like CSS files with
instant feedback.


So far the application understands the following CSS layout:

```
/*sass-start

Variables and functions can be placed in this tag.

this is how you set variables
$pop:46px; 
$background-color: red;

this is how to create functions
@pad($lop){
	padding: $lop;
	padding-bottom:$lop;
}
  

allways close the sass-start tag
sass-start*/ 
 

//first
#first {

	border: $pop; 
	padding: @pad(12px); 

	//second
	#second {
	@extend;
	color: purple; 
	border: 5px;

		//third
		#third {
			@extend; 
			color: $background-color;
			padding:9px;
 
			//fourth
			#fourth {
				@extend; 
				margin:5px; 
			}
		}
	}

}
 

/* this is how to tell the editor the css markup is finished */
/*sass-complete*/
```

Please note, the ```/*sass-start*/``` and ```/*sass-complete*/```, these tags are needed for the css processing to work correctly.
The CSS Editor recognises up to 4 levels of nesting. You can also extend the parent block inside a nested block.


##Requirements
*Windows 7+
*.NET 4.5


##Built With
*Visual Studio 2015


## Authors
* **Wayne Clarke** - [CSS Editor](https://github.com/Wayne-Clarke/CSS-Editor)


## License
This project is licensed as Freeware [LICENSE.md](LICENSE.md) file for details


