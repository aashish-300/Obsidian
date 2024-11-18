@Scope("singleton")
- default scope
- reference to single bean

@Scope("prototype")
- new instance is created every time bean is referenced

@Scope("session")
- a new instance is created once per uses session - web environment only

@Scope("request")
- a new instance is created once per request - web environment only
