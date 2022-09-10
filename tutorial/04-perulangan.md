## Perulangan

Diberikan sebuah kasus, untuk menampilkan angka 1 sampai 100. Akan sangat merepotkan jika kita harus mengetika seperti berikut:

```js
console.log(1)
console.log(2)
console.log(3)
...
console.log(100)
```

Untuk alternatifnya, kita bisa menggunakan _perulangan_.

### Perulangan _while_

Perulangan _while_ ditulis dengan sintaks berikut:

```js
while (kondisi) {
  // do something
}
```

Ketika `kondisi` bernilai _true_, maka `do something` akan dilakukan secara berulang.

```js
while (1 < 10) {
  console.log(i); // 1 sampai 9
  i++;
}
```

### Perulangan _do...while_

Perulangan dengan _do...white_ ditulis dengan sintaks

```js
do {
  // do something
} while (kondisi);
```

Perulangan dengan bentuk seperti di atas, akan menjalan `do something` terlebih dahulu tanpa mengecek kebenaran `kondisi`. Sebagai contoh

```js
let i = 0;
do {
  console.log(i);
  i++;
} while (i < 10);
```

Output di atas berupa angka 0 sampai 9.

### Perulangan _for_

Perulangan `for` lebih kompleks, tetapi sering digunakan.

```js
for (awal; kondisi; langkah) {
  // do something
}
```

Sebagai contoh:

```js
for (let i = 0; i < 5; i++) {
  console.log(i); // 0, 1, 2, 3, 4
}
```
