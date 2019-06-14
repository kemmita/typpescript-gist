```ts
//The below syntax will create a getter and setter for the name var in the class. public access modifier is needed for this.
class Machine{
    constructor(public name: string){}
}
const m = new Machine('Vehicle');
console.log(m.name);

```
