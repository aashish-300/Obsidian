
```
@Component(...)  
export class UserProfile {  
userId = input<number>();  
  
userService = inject(UserService);  
  
user = resource({  
request: this.userId,  
loader: async ({request: id}) => await userService.getUser(id),  
});  
}
```