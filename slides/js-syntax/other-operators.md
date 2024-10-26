#### JavaScript
### Autres opérateurs

<div class="r-stack">

<div class="fragment fade-out" data-fragment-index="1">

* Opérateur `typeof` pour déterminer le type d'une expression :
  `number`, `string`, `boolean`, `bigin`, `function`, `object`, `symbol` ou `undefined`

```javascript
console.log(typeof 42);                  // number 
console.log(typeof '42');                // string
console.log(typeof true);                // boolean
console.log(typeof 42n);                 // bigint
console.log(typeof (() => 42));          // function
console.log(typeof {});                  // object
console.log(typeof Symbol('42'));        // symbol
console.log(typeof undefined);           // undefined
console.log(typeof null);                // object
```

</div>

<div class="fragment fade-in-then-out" data-fragment-index="1">

* Opérateur ternaire

```javascript
const msg = new Date().getHours() > 12 ? 'Bonjour' : 'Bonsoir';
console.log(msg);
```
</div>

<div class="fragment fade-in-then-out">

* Opérateur de chaînage optionnel

```javascript
const person1 = { name: 'John' };
const person2 = null;
console.log(person1?.name);     // John
console.log(person2?.name)      // undefined
```

```javascript error
console.log(person2.name);      // TypeError
```
</div>

<div class="fragment">

* Opérateur de coalescence des nuls

```javascript
const nameDefault = 'John';
const nameNull = null;
const nameUndefined = undefined;
console.log(nameNull);                          // null
console.log(nameUndefined);                     // undefined
console.log(nameNull ?? nameDefault);           // John
console.log(nameUndefined ?? nameDefault)       // undefined
```

</div>

</div>
