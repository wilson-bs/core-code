## Answers Wednesday 26/01/2022
### 1 - [Valid Parentheses](https://www.codewars.com/kata/52774a314c2333f0a7000688)
```js
function validParentheses(parens) {
  var cont = 0;
  var cont2 = 0;
  var parentheses = parens.split('');
  
  if((parentheses[0] == ')') || (parentheses[parentheses.length-1] == '(')){
    return false;
  }else {
    
  for(var i=0;i<parentheses.length; i++){
    if(parentheses[i] == '('){
      cont ++;
    } else if(parentheses[i] == ')') {
      cont2 ++;
    }
  }
  if(cont != cont2) {
   return false; 
  }else {
    return true;
    }
  }
}
```

### 2 - [Convert string to camel case](https://www.codewars.com/kata/517abf86da9663f1d2000003)
```js
function toCamelCase(str){
  var msg = str.split('');
  var camelWord = '';
  for(var i=0;i<msg.length;i++){
    if(msg[i]=='_'|| msg[i]=='-'){   
    camelWord += msg[i+1].toUpperCase();
      i++;
 }else if(msg[i] != '_' && msg[i]!='-'){
    camelWord += msg[i];
 }
  }
  return camelWord;
}
```

### 3 - [Unique In Order](https://www.codewars.com/kata/54e6533c92449cc251001667)
```js
var uniqueInOrder = function (iterable) {
  var arrayIterable = Array.from(iterable);
  var result = [];

  for (var i = 0; i < arrayIterable.length; i++) {
    if (arrayIterable[i] != arrayIterable[i + 1]) {
      result.push(arrayIterable[i]);
    }
  }

  return result;
}
```