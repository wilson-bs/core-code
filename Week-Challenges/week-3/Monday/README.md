## Answers Monday 24/01/2022
### 1 - [Who likes it?](https://www.codewars.com/kata/5266876b8f4bf2da9b000362)
```js
function likes(names) {
  // TODO
  var msg = '';
  if(names.length == 0) {
    msg = 'no one likes this';
  }
  if(names.length == 1) {
    msg = names[0] + ' likes this';
  }
  if(names.length == 2) {
    msg = names[0] + ' and ' + names[1] + ' like this';
  }
  if(names.length == 3) {
    msg = names[0] + ', ' + names[1] + ' and ' + names[2] + ' like this';
  }
  if (names.length >= 4) {
      let res = 0;
      res = names.length - 2;
      msg = names[0] + ', ' + names[1] + ' and ' + res + ' others like this';
  }
  return msg;
}
```

### 2 - [Bit Counting](https://www.codewars.com/kata/526571aae218b8ee490006f4)
```js
var countBits = function(n) {
  var result = 0;
  result = n.toString(2);
  var total = 0;
  
  for(var i = 0; i<result.length;i++) {
    if(parseInt(result[i]) == 1){
      total += parseInt(result[i]);
    }  
  }
  return total;
};
```

### 3 - [Decode the Morse code ](https://www.codewars.com/kata/54b724efac3d5402db00065e)
```js
decodeMorse = function(morseCode){
  var og_msg = '';
  var wd_msg = '';
  var msg = '';
  
  og_msg = morseCode.trim().split('   ');
  wd_msg = og_msg.join('  ');
  
  
  for (var i = 0; i<wd_msg.split(' ').length; i++){
    if(MORSE_CODE[wd_msg.split(" ")[i]] == undefined) {
      msg += " ";
    }else {      
    msg += MORSE_CODE[wd_msg.split(" ")[i]];
    }
  }
  return msg;
}
```