`linkedSignal` clearly expresses the relationship between `options` and `choice` without resorting to an `effect` usage.
```
const options = signal(['apple', 'banana', 'fig']);  
  
// Choice defaults to the first option, but can be changed.  
const choice = linkedSignal(() => options()[0]);  
console.log(choice()); // apple  
  
choice.set('fig');  
console.log(choice()); // fig  
  
// When options change, choice resets to the new default value.  
options.set(['peach', 'kiwi']);  
console.log(choice()); // peach
```