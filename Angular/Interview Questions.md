1. Ahead Of Time(AOT) vs Just In Time(JIT)
	- AOT precompiles before they are loaded in the browser.
	- JIT compiles angular templates during runtime right in the client's browser
2. Explain what an ngModule is.
   - An NgModule is a class marked by the `@NgModule` decorator. This decorator accepts _metadata_ that tells Angular how to compile component templates and configure dependency injection.
3. [`Services and dependency injection`](https://www.crsinfosolutions.com/services-and-dependency-injection-in-angular-interview-questions/#:~:text=A%20service%20in%20Angular%20is,modularity%20within%20your%20Angular%20application)
4. forwardRef in Angular dependency
	- The `forwardRef` function is used to handle circular dependencies, where two classes depend on each other. It allows you to refer to a class that is not yet defined or available at the time of declaration
```
	constructor(@Inject(forwardRef(() => SomeService)) private someService:    
	SomeService) {}
```