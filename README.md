#CSS Editor.
With this application you can edit CSS files using functions and variables.
Currently the editor is in the beta stage so its not ready for production use but you may
use it and offer any feedbacks. 

The purpose of this application is to offer a way to pre-process sass like CSS files with
instant feedback.


So far the application understands the following CSS layout:

```
/* 
Insert variables and functions here!
$pop:46px; 

@pad($lop){
	padding: $lop;
	padding-bottom:$lop;
}

@import "c:\Users\bobby\desktop\testCss.css"  
start */ 
 

#first {

	border: $pop; 
	padding: @pad(12px); 

	#second {
	@extend;
	color: purple; 
	border: 5px;

		#third {
			@extend; 
			color: blue;
			padding:9px;
 
			#fourth {
				@extend; 
				margin:5px; 
			}
		}
	}

}
 
/*end*/
```

Please note, the ```/*start*/``` and ```/*end*/``` tags are needed for the processing to work correctly.
The CSS Editor recognises up to 4 levels of nesting. You can also extend the parent block inside a nested block.


##Requirements
*Windows 7+
*.NET 4.5


##Built With
*Visual Studio 2015


## Authors
* **Wayne Clarke** - [CSS Editor](https://github.com/Wayne-Clarke/CSS-Editor)


## License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details


