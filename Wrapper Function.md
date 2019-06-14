1. Wrapper functions a re a bit like delegates where we can pass data and a selected function to another funcitonto provide
dynamic output
```ts
let calc = (calcFunc: Function, ...nums: number[]): Function =>{
    return calcFunc(nums);
};

let add = (nums: number[]): number =>{
  let total = 0;
  nums.forEach(number =>{
      total += number;
  });
  return total;
};

let multiply = (nums: number[]): number =>{
    let total = 1;
    nums.forEach(number =>{
        total *= number;
    });
    return total;
};

console.log(calc(add,5,5));
console.log(calc(multiply,5,5));
```
