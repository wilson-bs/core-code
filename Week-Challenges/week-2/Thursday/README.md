## Answers Thursday 20/01/2022
### 1 - [Exclamation marks series #2: Remove all exclamation marks from the end of sentence](https://www.codewars.com/kata/57faece99610ced690000165)
```js
function remove (string) {
  var clean =[];
  for (var i = string.length-1; i => 0; i--){
    if(string[i] != '!'){ 
      clean.push(string.slice(0,i+1));
      return clean.join('');
    }
  }
}
```

### 2 - [Vowel remover](https://www.codewars.com/kata/5547929140907378f9000039)
```js
function shortcut (str) {
  const vocales = /[aeiou]+/g;
  let resultado;
  resultado = str.replace(vocales,'');
  return resultado;
}
```

### 3 - [Rock Paper Scissors!](https://www.codewars.com/kata/5672a98bdbdd995fad00000f)
```js
const rps = (p1, p2) => {
  if(p1 === p2) {
    return "Draw!";
  }
  if((p1=='scissors') && (p2!='rock')) {
    return 'Player 1 won!';
  } else if((p1=='paper') && (p2!='scissors')) {
    return 'Player 1 won!';
  }else if((p1=='rock') && (p2!='paper')) {
    return 'Player 1 won!';
  }
  return 'Player 2 won!';
};
```

### 4 - [Persistent Bugger.](https://www.codewars.com/kata/55bf01e5a717a0d57e0000ec)
```js
function persistence(num) {
  for (var i = 0; num > 9; i++) {
    num = num.toString().split("").reduce((firstN,secondN) => firstN * secondN);
  } return i;
}
```

### 5 - ✨Complete your 1st [Core Challenge](https://corecode.notion.site/Mission-Statement-666f515d76084c8e8c996b473b4d6317). This is one of the requirements for the certification, where you'll boost your dev professional-brand.
> I am Wilson, a junior C++ software developer. I’ve been developing solutions in this language for a year now, including SQL, HTML & Javascript. I’m looking forward to growing as a professional, learning new technologies to open opportunities for work outside Guatemala. I´m a committed person who believes that every goal it’s possible to achieve with passion and constancy, and I continue working to prove it.