## Function

### Deklarasi _function_

Dalam mendeklarasikan `function`, diperlukan

- nama dari function,
- parameter-parameter, dan
- statement yang dijalankan di dalam blok kode `{ ... }`. Sebagai contoh:

```js
function jumlah(a, b) {
  return a + b;
}

console.log(jumlah()); // NaN
console.log(jumlah(1, 2)); // 3
```

Fungsi `jumlah` membutuhkan 2 parameter `a` dan `b`. Jika kita menjalankan fungsi tersebut tanpa menggunakan parameter, maka akan mengembalikan nilai `NaN`.

Selain dengan cara tersebut, kita juga bisa mendeklarasikan fungsi seperti ini:

```js
const nameFunction = function () {
  // do something
};
```

Sebagai contoh:

```js
const jumlah = function (a, b) {
  return a + b;
};

console.log(jumlah(2, 3)); // 5
```

## Arrow Function

Penulisan sintaks function juga dapat dilakukan sebagai berikut:

```js
const functionName = (parameter) => {
  // do something
};
```

Penulisan dengan model tersebut dinamakan _arrow function_. Sebagai contoh:

```js
const jumlah = (a, b) => {
  return a + b;
};

console.log(jumlah(2, 4)); // 6
```
