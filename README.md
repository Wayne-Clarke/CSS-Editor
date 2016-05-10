#CSS Editor.
With this application you can edit CSS files using functions and variables.
Currently the editor is in the beta stage so its not ready for production use but you may
use it and offer any feedbacks. 

The purpose of this application is to offer a way to pre-process sass like CSS files with
instant feedback.



So far the application understands the following CSS layout:

/* 
Insert variables and functions here!
$pop:46px; 

@pad($lop){
	padding: $lop;
	padding-bottom:$lop;
}

@import "c:\Users\jtones\desktop\testCss.css"  
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


Please note, the /*start*/ and /*end*/ tags are needed for the processing to work correctly,


Requirements
Windows 7+
.NET 4.5
