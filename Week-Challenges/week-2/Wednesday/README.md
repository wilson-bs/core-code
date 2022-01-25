## Answers Wednesday 19/01/2022
### 1 - [Holiday VIII - Duty Free](https://www.codewars.com/kata/57e92e91b63b6cbac20001e5)
```js
function dutyFree(normPrice, discount, hol){
  var holprice = 0;
  holprice = hol / (normPrice * (discount/100))
  return parseInt(holprice);
}
```

### 2 - [Twice as old](https://www.codewars.com/kata/5b853229cfde412a470000d0)
```js
function twiceAsOld(dadYearsOld, sonYearsOld) {
  var age = 0;
  var twice = 0;
  
  twice = sonYearsOld * 2;
  if (twice < dadYearsOld) {
    age = dadYearsOld - twice;
  }else {
    age = twice - dadYearsOld;
  }
  return age;
}
```

### 3 - [Valid Spacing](https://www.codewars.com/kata/5f77d62851f6bc0033616bd8)
```js
function validSpacing(s) {
  if (s == "")
    return true
  else
    return !s.split(" ").includes("")
}
```

### 4 - [Fake Binary](https://www.codewars.com/kata/57eae65a4321032ce000002d)
```js
function fakeBin(x){
  var ogArray;
  
  ogArray = x.split('');
  for (var i = 0; i < ogArray.length; i++) {
    if(ogArray[i] < 5) {
      ogArray[i] = '0';
    }
    else {      
    ogArray[i] = '1';
    }
  }
  return ogArray.join('');
}
```