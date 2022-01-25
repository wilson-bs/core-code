## Answers Tuesday 18/01/2022
### 0 - Watch [this](https://www.youtube.com/watch?v=cEBkvm0-rg0) video
--Done
### 1 - [Multiply](https://www.codewars.com/kata/50654ddff44f800200000004)
```js
function multiply(a, b){
  return a * b;
}
```
### 2 - [ASCII Total](https://www.codewars.com/kata/572b6b2772a38bc1e700007a)
```js
function uniTotal (string) {
// total up dem unicodes!
 
let total = 0;
  
for (var i = 0; i < string.length; i++) {
total += string.charCodeAt(i)
}
  return total;
}
```

### 3 - [get character from ASCII Value](https://www.codewars.com/kata/55ad04714f0b468e8200001c)
```js
function getChar(c){
  // ...
  valor = String.fromCharCode(c);
  return valor;
}
```

### 4 - [Binary Addition](https://www.codewars.com/kata/551f37452ff852b7bd000139)
```js
function addBinary(a,b) {
  let suma = 0;
  let binary;
  suma = a + b;
  binary = suma.toString(2);
  return binary;
}
```

### 5 - [Student's Final Grade](https://www.codewars.com/kata/5ad0d8356165e63c140014d4)
```js
function finalGrade (exam, projects) {
  var fGrade = 0;
  if((exam > 90) || (projects > 10)) {
    fGrade = 100;
  }
  else if((exam > 75) && (projects >= 5)) {
    fGrade = 90;
  }
  else if((exam > 50) && (projects >= 2)) {
    fGrade = 75;
  }
  else if ((exam < 50) && (projects < 2)) {
    fGrade = 0;
  }
  return fGrade;// final grade
}
```