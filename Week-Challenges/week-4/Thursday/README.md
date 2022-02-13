## Answers Thursday 03/02/2022
### 1 - [Detect Pangram](https://www.codewars.com/kata/545cedaa9943f7fe7b000048)
```js
function isPangram(string) {
  const alphabeth = "abcdefghijklmnopqrstuvwxyz".split("");

  const otherString = string.toLowerCase().replace(/\s|\./g, "").split("");

  for (let i = 0; i < alphabeth.length; i++) {
    if (!otherString.includes(alphabeth[i])) return false;
  }

  return true;
}
```

### 2 - [Find the missing letter](https://www.codewars.com/kata/5839edaa6754d6fec10000a2)
```js
function findMissingLetter(array) {
    var missingLetter = '';
    var codeArray = array.join('').charCodeAt(0);
    for (var j = 0; j < array.length; j++) {
        if (array.join('').charCodeAt(j) != codeArray + j){
            missingLetter = String.fromCharCode(codeArray + j);
            return missingLetter;
        }
    }
}
```

### 3 - [Find the unique number](https://www.codewars.com/kata/585d7d5adb20cf33cb000235)
```js
function findUniq(arr) {
  let values = {};
  arr.forEach((element) => {
    if (values[element] == undefined){
      values[element] = 1;
    }else {
      values[element]++;
    }
  });
  for (const key in values) {
    if (values[key] == 1) return key * 1;
  }
}
```

### 4 - [Reverse or rotate?](https://www.codewars.com/kata/56b5afb4ed1f6d5fb0000991)
```js
function revrot(str, sz) {
  if (sz <= 0 || sz > str.length) return "";
  //Not finished
  }
```

### 5 - [What's Your Poison?](https://www.codewars.com/kata/58c47a95e4eb57a5b9000094)
```js
function find(rats) {
  return rats.reduce((a,b) => a + Math.pow(2, b), 0);
}
```

### 6 - ✨Complete your 3rd [Core Challenge](https://corecode.notion.site/GitHub-Boost-Guide-167914056cff4522886a78756f659e47). This is one of the requirements for the certification, where you'll boost your dev professional-brand.
 ### 💻 [My GitHub](https://github.com/wilson-bs)
