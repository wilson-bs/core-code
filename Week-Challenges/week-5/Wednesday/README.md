## Answers Wednesday 09/02/2022
### 1 - [Duplicate Encoder Using Typescript](https://www.codewars.com/kata/54b42f9314d9229fd6000d9c/train/typescript)
```js
export function duplicateEncode(word: string){
    var encode = word.toLowerCase()
    .split('')
    .map( function (act, prev, arr) {
      return arr.indexOf(act) == arr.lastIndexOf(act) ? '(' : ')'
    })
    .join('');
  return encode;
}
```

### 2 - [Find the odd int Using Typescript](https://www.codewars.com/kata/54da5a58ea159efa38000836/train/typescript)
```js
export const findOdd = (xs: number[]): number => {
    return xs.reduce( (num,rep)=> num^rep);
};
```

### 3 - [Which are in? Using Typescript](https://www.codewars.com/kata/550554fd08b86f84fe000a58/train/typescript)
```js
```

### 4 - Sums of Parts Using Typescript
```js
export function partsSums(ls: number[]): number[] {
  let result = ls.reduce((a, b) => a + b, 0);
  let resultArr = [];
  let x = 0;
  if(ls.length === 0) {
    return [0];
  }
  for(let i = 0; i <= ls.length; i += 1) {
    resultArr.push(result);
    x = ls[i];
    result -= x;
  }  
  return resultArr;
}
```

### 5 - [Consecutive strings Using Typescript](https://www.codewars.com/kata/56a5d994ac971f1ac500003e)
```js
export function longestConsec(strarr: string[], k: number): string {
    let result = strarr.length;
    if(result == 0 || k > result || k <= 0) return '';
    
    let totalnum:string = '', temp: string = '';
    strarr.map((e, i, starrr) => {
        temp = starrr.slice(i, i+k).join("");
        if(temp.length > totalnum.length) totalnum = temp;
    })
    return totalnum;
}
```