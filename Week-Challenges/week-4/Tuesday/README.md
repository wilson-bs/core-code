## Answers Tuesday 01/02/2022
### 1 - This [link](https://www.typescriptlang.org/docs/handbook/intro.html) is nice to have and read
 * Done ✅

### 2 - [Typescript object type](https://typescript-exercises.github.io/#exercise=1)
```typescript
/*Exercise:
    Given the data, define the interface "User" and use it accordingly.
*/

export type User = { name: string; age: number; occupation: string };

export const users: User[] = [
    {
        name: 'Max Mustermann',
        age: 25,
        occupation: 'Chimney sweep'
    },
    {
        name: 'Kate Müller',
        age: 23,
        occupation: 'Astronaut'
    }
];

export function logPerson(user: User) {
    console.log(` - ${user.name}, ${user.age}`);
}

console.log('Users:');
users.forEach(logPerson);
```

### 3 - Read [this](https://blog.logrocket.com/types-vs-interfaces-in-typescript/)
* Done ✅

### 4 - [Typescript union types](https://typescript-exercises.github.io/#exercise=2)
```typescript
/*Exercise:
    Type "Person" is missing, please define it and use
    it in persons array and logPerson function in order to fix
    all the TS errors.
*/

interface User {
    name: string;
    age: number;
    occupation: string;
}

interface Admin {
    name: string;
    age: number;
    role: string;
}

export type Person = User | Admin;

export const persons: Person[] /* <- Person[] */ = [
    {
        name: 'Max Mustermann',
        age: 25,
        occupation: 'Chimney sweep'
    },
    {
        name: 'Jane Doe',
        age: 32,
        role: 'Administrator'
    },
    {
        name: 'Kate Müller',
        age: 23,
        occupation: 'Astronaut'
    },
    {
        name: 'Bruce Willis',
        age: 64,
        role: 'World saver'
    }
];

export function logPerson(user: Person) {
    console.log(` - ${user.name}, ${user.age}`);
}

persons.forEach(logPerson);
```

### 5 - [Typescript in operator](https://typescript-exercises.github.io/#exercise=3)
```typescript
/*
Exercise:
    Fix type errors in logPerson function.

    logPerson function should accept both User and Admin
    and should output relevant information according to
    the input: occupation for User and role for Admin.
*/

interface User {
    name: string;
    age: number;
    occupation: string;
}

interface Admin {
    name: string;
    age: number;
    role: string;
}

export type Person = User | Admin;

export const persons: Person[] = [
    {
        name: 'Max Mustermann',
        age: 25,
        occupation: 'Chimney sweep'
    },
    {
        name: 'Jane Doe',
        age: 32,
        role: 'Administrator'
    },
    {
        name: 'Kate Müller',
        age: 23,
        occupation: 'Astronaut'
    },
    {
        name: 'Bruce Willis',
        age: 64,
        role: 'World saver'
    }
];

export function logPerson(person: Person) {
    let additionalInformation: string;
    if ('role' in person) {
        additionalInformation = person.role;
    } else {
        additionalInformation = person.occupation;
    }
    console.log(` - ${person.name}, ${person.age}, ${additionalInformation}`);
}

persons.forEach(logPerson);
```


### 6 - [Find the odd int](https://www.codewars.com/kata/54da5a58ea159efa38000836)
```js
function findOdd(A) {
  var res = 1;
  var result = 0;
  A.sort((a, b) => a - b).forEach((value, index, array) => {
    if (value == array[index + 1]) {
      res++;
    } else {
      if (res % 2 != 0) {
        result = value;
      }
      res = 1;
    }
  });
  return result;
}
```

### 7 - [Stop gninnipS My sdroW!](https://www.codewars.com/kata/5264d2b162488dc400000001)
```js
function spinWords(string) {
  return string
    .split(" ")
    .reduce((previous, actual) => {
      return `${previous} ${
        actual.length >= 5 ? actual.split("").reverse().join("") : actual
      }`;
    }, "").trim();
}
```