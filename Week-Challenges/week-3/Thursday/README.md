## Answers Thursday 27/01/2022
### 1 - [Fold an array](https://www.codewars.com/kata/57ea70aa5500adfe8a000110)
```js
function foldArray(array, runs) {
  var newArray = Array.from(array);
    while (runs > 0) {
      var result = [];
      while (newArray.length > 1) {
        let firstElement = newArray.shift();
        let lastElement = newArray.pop();
        result.push(firstElement + lastElement);
      }
      newArray = [...result, ...newArray];
      runs--;
    }
    return newArray;
}
```

### 2 - [Encrypt this!](https://www.codewars.com/kata/5848565e273af816fb000449)
```js   
var encryptThis = function(text) {
 return text.split(' ').map(
   q => {
      if (q.length==1) return q.charCodeAt(0)
      if (q.length==2) return `${q[0].charCodeAt(0)}${q[1]}`
      if (q.length==3) return `${q[0].charCodeAt(0)}${q.slice(-1)}${q[1]}`
      if (q.length > 3) return `${q[0].charCodeAt(0)}${q.slice(-1)}${q.slice(2,-1)}${q[1]}`  
  }).join(' ');
}
```

### 3 - [Format a string of names like 'Bart, Lisa & Maggie'.](https://www.codewars.com/kata/53368a47e38700bd8300030d)
```js
function list(names){
  return names
    .reduce((previous, current, index, array) => {
      return `${previous}${index != array.length - 1 ? ", " : " & "}${current.name}`;
    }, "")
    .trim().slice(2);
}
```
### 4 - ✨Complete your 2nd [Core Challenge](https://corecode.notion.site/LinkedIn-Boost-5974abb0f917458ea235d3288ac6c7d3). This is one of the requirements for the certification, where you'll boost your dev professional-brand.
 #### 🏅[My Linkedin Profile](https://www.linkedin.com/in/wilson-barrientos/)
