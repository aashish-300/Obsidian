- Pipes are defined using the pipe “|” symbol.

Types of pipes
- pure pipes
	- Pure pipes in angular are the pipes that execute when it detects a __pure change__ in the input value.
	```
	import { Component } from '@angular/core';
	@Component({
	  selector: 'app-root',
	  templateUrl: 'app.component.html',
	  styleUrls: ['./app.component.css']
	})
	export class AppComponent {
		  user = { name:'Rohit', age: 23};
		}
	```
	 - here changes in user.age value doesn't detect change as object reference is same. To detect changes angular has to detect deep changes which is not pure.
	 
- impure pipes
	```
	@Pipe({
	  name: 'myPipe', 
	  pure: false       
		})
		export class MyPipe {...}
	```
     - Now, myPipe will execute on every change.