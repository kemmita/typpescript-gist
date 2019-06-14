1. Decorator are used to attach functionlity to a class when it is executed. The function below will run first when 
the class below it is called.
```ts
let target = (Target) =>{
  console.log(Target);
};

@target
class MyClass {
    name: string;
    age: number;
}

```
