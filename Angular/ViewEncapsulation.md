```
	enum [ViewEncapsulation](https://angular.dev/api/core/ViewEncapsulation) { 
	Emulated: ViewEncapsulation.Emulated; 
	None: ViewEncapsulation.None; 
	ShadowDom: ViewEncapsulation.ShadowDom;
}
```

Emulated
- default set to emulated
- specific html attribute is set to css
- css only works in which component css is declared

None
- works as global css

ShadowDom
- creates a shadowRoot inside html 
- global css is not effected inside component
- css inside component is not effected globally
