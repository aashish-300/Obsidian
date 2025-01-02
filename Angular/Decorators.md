In Angular, decorators are functions that are used to ****modify the behavior of classes and their members****. They provide a ****way to add metadata**** or apply transformations to code elements. In Angular, decorators are extensively used to define components, services, directives, pipes, modules, and more

Types of decorators
1. class decorators:
	- Class decorators are applied to classes to modify their behavior or metadata. The examples include @Component, @Directive and @NgModule.
2.  Property decorators: 
	- Property decorators are applied to the class properties and are commonly used to modify the properties within the classes. For example, @Input decorator makes a property as an input binding, allowing it to bound to the external data.
3. Method decorators:
   - Method decorators are applied to the class methods and modify their behavior or add additional functionalities. For example, @HostListener allows us to listen for events on a method.
4. Parameter decorators:
   - The Parameter decorators are used for parameters inside class constructors. The parameter decorators provide additional information about constructor parameters. For example, The @Inject decorator allows to specify dependencies for dependency injection.