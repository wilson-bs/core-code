## Answers Monday 07/02/2022
### 1 - Read [this](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html) from The primitives: string, number and boolean to Differences Between Type Aliases and Interfaces section
 * Done ✅

### 2 - [Square(n) Sum Using Typescript](https://www.codewars.com/kata/515e271a311df0350d00000f/train/typescript)
```js
export function squareSum(numbers: number[]): number {
   var sum = 0;

  for(var i = 0; i < numbers.length; i++) {
    sum += numbers[i] * numbers[i]; 
    }
  return sum;
}
```

### 3 - [Growth of a Population Using Typescript](https://www.codewars.com/kata/563b662a59afc2b5120000c6/train/typescript)
```js
export class G964 {

    public static nbYear = (p0, percent, aug, p) => {
        percent = percent / 100;
        let i = 0;
        while (p > p0) {
            p0 += p0 * percent + aug;
          i++;
        }
    return i;
    }
}
```

### 4 - [Mumbling Using Typescript](https://www.codewars.com/kata/5667e8f4e3f572a8f2000039/train/typescript)
```js
export function accum(s: string): string {
    var newString:string =
        s.split("").map((element, i) => {
            return element.toUpperCase() + element.toLowerCase().repeat(i);
        }).join("-");
    return newString;
}
```

### 5 - [A wolf in sheep's clothing Using Typescript](https://www.codewars.com/kata/5c8bfa44b9d1192e1ebd3d15/train/typescript)
```js
export function warnTheSheep(queue: string[]): string {
  if (queue.indexOf("wolf") != queue.length - 1) {
    let position:number = queue.length - queue.indexOf("wolf") - 1;
    return `Oi! Sheep number ${position}! You are about to be eaten by a wolf!`
  } else {
      queue.length - 1 - queue.indexOf("wolf");
      return "Pls go away and stop eating my sheep";
    }
}
```