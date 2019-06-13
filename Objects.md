1. Below we create an object and then loop through the object items

```ts
let student = {
  name: 'Russell',
  age: 29,
  career: 'Developer',
};

for (let studentKey in student) {
    console.log(studentKey)
}
```
