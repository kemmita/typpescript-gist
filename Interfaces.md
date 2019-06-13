1. Below we create an interface and then have an object implement that interface
```ts
//readonly is optional
interface ISerialKiller {
   readonly killerName: string,
   readonly bodyCount: number,
   readonly stillAlive: boolean,
   preview: {(x)}
}

const Gacey: ISerialKiller = {
    killerName: 'John W Gacey',
    bodyCount: 30,
    stillAlive: false,
    preview: () => {console.log(`Their name is ${killerName}, they had a body count of ${bodyCount}`)}
};


let {killerName} = Gacey;
console.log(killerName)
```

2. Below we extend interfaces by using inheritince 
```ts
interface ISerialKiller {
    readonly killerName: string,
    readonly bodyCount: number,
    readonly stillAlive: boolean
}

interface IVictim extends ISerialKiller{
    victimName: string,
    victimAge: number
}

const johnDoe: IVictim ={
    killerName: 'John W Gacey',
    bodyCount: 30,
    stillAlive: false,
    victimAge: 21,
    victimName: 'John Doe'
};
```

3. 
