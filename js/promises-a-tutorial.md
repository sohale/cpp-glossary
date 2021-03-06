remember three functions:
`new Promise(()=>{})`
`p.then(()=>{})`
`p.catch(()=>{})`

bonus:
`p.finally()`

Allinputs and outputs of Promise:

```javascript
var p1 = new Promise((resolve, reject)=>{
    BODY

    resolve(A2)
    reject(B3);

    throw C4;
    return D5;

    W6 = this;

    U7 = resolve(u);
    V8 = reject(v);

    return resolve(a);
    throw reject(b);
})
```

What happens to `C4`, `D5`?
What if we return after resolve?
what is we resolve twice?
or resolve, then reject?

When if `p`'s body is executed and then we attach a `.then()`?
What if we `.then()` a `p` and then `.then()` the same `p`?

* If the `p` is executed already, and then we `.then()` it, when will the `then()`ed clause be executed? For example:
```javascript
//in REPL mode of nodejs:
const p = new Promise((res, rej)=>{console.log('promise');});
//output is seen here
p.then((x)=>{console.log('then 1', x);})
//and then even:
p.then((x)=>{console.log('then 2', x);})
```

* If we call resolve inside a then:
```javascript
.then((x)=>{
    resolve(x);
})
```
then, is it necessarily a resolve of an outer promise?

* In what case we return the resolved?
```javascript
new Promise((res, rej)=>{
    return res(9);
});
```


### Answers

`return` is useless and pointless in the promise body. It is just about leaving the code block.
the return vaue from `resolve` is simpluy `undefined`.


(When we don't resolve)
If in promise body, we `throw`, it goes inot the catch. But if we `return`, it doesn't enter the `then()`.

If no `resolve()` or `reject()` yet, `throw` -> `catch`, but `return` -(NOT)-> `then()`.
