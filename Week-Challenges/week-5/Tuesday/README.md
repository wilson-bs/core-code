## Answers Tuesday 08/02/2022
### 1 - [A Rule of Divisibility by 13 Using Typescript](https://www.codewars.com/kata/564057bc348c7200bd0000ff)
```js

```

### 2 - [Playing with digits Using Typescript](https://www.codewars.com/kata/5552101f47fc5178b1000050)
```js
export class G964 {

  public static digPow = (n: number, p: number) => {
    let result: number = n.toString().split("")
      .reduce((prev, current) => {
          return prev + Math.pow(Number(current), p++);
    }, 0);
    return result % n ? -1 : result / n;
  }
}
```

### 3 - [Valid Braces Using Typescript](https://www.codewars.com/kata/5277c8a221e209d3f6000b56)
```js
export function validBraces(braces: string): boolean {
  let cont: number = 0;
  let allBraces = braces.split("");
  let result: boolean = false;
  for (let i = 0; i < allBraces.length; i++) {
    if (allBraces[i] == ")") {
      cont--;
      if (allBraces[i - 1] == "(") result = true;
    } else if (allBraces[i] == "}") {
      cont--;
      if (allBraces[i - 1] == "{") result = true;
    } else if (allBraces[i] == "]") {
      cont--;
      if (allBraces[i - 1] == "[") result = true;
    } else {
      cont++;
    }
    if (cont < 0) return false;
  }
  return result;
}
```

### 4 - [Tic-Tac-Toe Using Javascript](https://www.codewars.com/kata/5216a87cbf53a9c30f0000dc)
```js
```

### 5 - [Tic-Tac-Toe-like table Generator Using Javascript](https://www.codewars.com/kata/5b817c2a0ce070ace8002be0)
```js

```
