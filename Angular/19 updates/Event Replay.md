Event dispatch captures events during initial page load and replays them when the code responsible for handling the events is available. Event dispatch is the same [library](https://github.com/angular/angular/tree/main/packages/core/primitives/event-dispatch) that the Wiz team developed for Google Search

You can enable event replay feature in Angular by configuring your hydration provider:

For new projects the Angular CLI will generate this code by default  
```
bootstrapApplication(App, {  
  providers: [  
    provideClientHydration(withEventReplay())  
  ]  
});
```
