# typescript-tutorial

This is a _collection_ of `code` from a Youtube video of [Dave Gray](https://github.com/gitdagray) || [video link](https://www.youtube.com/playlist?list=PL0Zuz27SZ-6NS8GXt5nPrcYpust89zq_b)

You can also [check out](https://github.com/gitdagray/typescript-course) his Github page for details lessons.

## Jump to specific Chapter

- [typescript-tutorial](#typescript-tutorial)
  - [Jump to specific Chapter](#jump-to-specific-chapter)
    - [Chapter 1 - Introduction, Setup \& Config](#chapter-1---introduction-setup--config)
    - [Chapter 2 - Basic Types](#chapter-2---basic-types)
    - [Chapter 3 - Arrays, Tuples, Objects \& Enums](#chapter-3---arrays-tuples-objects--enums)

### Chapter 1 - Introduction, Setup & Config

```ts
let username = "Dave";
console.log(username);

let a: number = 12;
let b: string = "6";
let c: number = 2;

console.log(a / b);

console.log(c * b);
```

### Chapter 2 - Basic Types

```ts
let myName: string = "Dave";
let meaningOfLife: number;
let isLoading: boolean;
let album: any;

myName = "John";
meaningOfLife = 42;
isLoading = true;
album = 5150;

const sum = (a: number, b: string) => {
  return a + b;
};

let postId: string | number;
let isActive: number | boolean;

let re: RegExp = /\w+/g;
```

### Chapter 3 - Arrays, Tuples, Objects & Enums

```ts
let stringArr = ["one", "hey", "Dave"];

let guitars = ["Strat", "Les Paul", 5150];

let mixedData = ["EVH", 1984, true];

stringArr[0] = "John";
stringArr.push("hey");

guitars[0] = 1984;
guitars.unshift("Jim");

let test = [];
let bands: string[] = [];
bands.push("Van Halen");

// Tuple
let myTuple: [string, number, boolean] = ["Dave", 42, true];

let mixed = ["John", 1, false];

myTuple[1] = 42;

// Objects
let myObj: object;
myObj = [];
console.log(typeof myObj);
myObj = bands;
myObj = {};

const exampleObj = {
  prop1: "Dave",
  prop2: true,
};

exampleObj.prop1 = "John";

interface Guitarist {
  name?: string;
  active: boolean;
  albums: (string | number)[];
}

let evh: Guitarist = {
  name: "Eddie",
  active: false,
  albums: [1984, 5150, "OU812"],
};

let jp: Guitarist = {
  active: true,
  albums: ["I", "II", "IV"],
};

const greetGuitarist = (guitarist: Guitarist) => {
  if (guitarist.name) {
    return `Hello ${guitarist.name.toUpperCase()}!`;
  }
  return "Hello!";
};

console.log(greetGuitarist(jp));

// Enums
// "Unlike most TypeScript features, Enums are not a type-level addition to JavaScript but something added to the language and runtime."

enum Grade {
  U = 1,
  D,
  C,
  B,
  A,
}

console.log(Grade.U);
```
