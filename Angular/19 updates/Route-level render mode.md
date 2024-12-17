In v19, we provide a new interface called `ServerRoute` which allows you to configure whether the individual routes should be server-side rendered, prerendered, or rendered on the client side:

```
export const serverRouteConfig: ServerRoute[] = [  
{ path: '/login', mode: RenderMode.Server },  
{ path: '/dashboard', mode: RenderMode.Client },  
{ path: '/**', mode: RenderMode.Prerender },  
];
```

```
export const routeConfig: ServerRoute = [{  
path: '/product/:id',  
mode: 'prerender',  
async getPrerenderPaths() {  
const dataService = inject(ProductService);  
const ids = await dataService.getIds(); // ["1", "2", "3"]  
return ids.map(id => ({ id })); // `id` is used in place of `:id` in the route path.  
},  
}];
```