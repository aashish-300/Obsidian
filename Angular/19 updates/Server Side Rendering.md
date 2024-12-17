To create a new project with SSR, run:
```
ng new --ssr
```

To Add SSR to an existing project
```
ng add @angular/ssr
```

These commands create and update application code to enable SSR and adds extra files to the project structure.

```
my-app
|-- server.ts                       # application server
└── src
    |-- app
    |   └── app.config.server.ts    # server application configuration
    └── main.server.ts              # main server application bootstrapping
```