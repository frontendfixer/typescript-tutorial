# typescript-tutorial

This is a _collection_ of `code` from a Youtube video of [Dave Gray](https://github.com/gitdagray) || [video link](https://www.youtube.com/playlist?list=PL0Zuz27SZ-6NS8GXt5nPrcYpust89zq_b)

You can also [check out](https://github.com/gitdagray/typescript-course) his Github page for details lessons.

## Jump to specific Chapter

- [typescript-tutorial](#typescript-tutorial)
  - [Jump to specific Chapter](#jump-to-specific-chapter)
    - [Chapter 1 - Introduction, Setup \& Config](#chapter-1---introduction-setup--config)
    - [Chapter 2 - Basic Types](#chapter-2---basic-types)

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
