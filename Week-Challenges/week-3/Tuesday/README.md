## Answers Tuesday 25/01/2022
### 1 - [Your order, please](https://www.codewars.com/kata/55c45be3b2079eccff00010f)
```js
function order(words) {
  var digit = /\d/;
  var inOrder = [];

  words.split(" ").forEach((word) => {
    var newOrder = parseInt(word.match(digit));
    inOrder[newOrder - 1] = word;
  });

  return inOrder.join(" ");
}
```

### 2 - [Counting Duplicates](https://www.codewars.com/kata/54bf1c2cd5b56cc47f0007a1)
```js
function duplicateCount(text) {
    var letter = text.toLowerCase();
    var newCount = {};
    var total = 0;
    for (var i = 0; i < letter.length; i++) {
        if (!newCount[letter[i]]){
            newCount[letter[i]] = 1;
        }
        else if (newCount[letter[i]] < 2) {
            newCount[letter[i]] += 1;
            total++;
        }
    }
    return total;
}
```

### 3 - [Simple Pig Latin](https://www.codewars.com/kata/520b9d2ad5c005041100000f)
```js

```
