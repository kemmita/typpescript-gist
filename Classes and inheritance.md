```ts
//below we create a class like we would do in JS
class Machine{
    public weight: number;
    constructor(weight: number){
        this.weight = weight;
    }
    public demo(){
        console.log(`This machine weighs ${this.weight} pounds.`);
    }
}
let m = new Machine(19);
console.log(m.demo());

//Here we inherit from a class like we do in js
class Car extends Machine{
    public vehicleName: string;

    constructor(weight:number, vehicleName) {
        super(weight);
        this.vehicleName = vehicleName;
    }

    public description(){
        console.log(`Vehicle ${this.vehicleName} weighs ${this.weight}`);
    }
}

let c = new Car(2200, '4 door Jeep');
console.log(c.description());

```

