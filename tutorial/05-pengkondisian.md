## Pengkondisian

Dalam menjalankan perintah, seringkali kita membutuhkan kondisi apakah perintah tersebut dijalankan atau tidak. Dalam kasus tersebut, kita dapat menggunakan pengkondisian, salah satunya `if`.

### Pernyataan _if_

Pernyataan `if` mengecek suatu kondisi. Jika kondisi tersebut `true`, maka blok kode di dalam `if` akan dijalankan. Sebagai contoh:

```js
let usia = 18;
if (usia > 17) {
  console.log('bisa buat KTP');
}
```

Karena benar bahwa `18 > 17`, maka blok kode `console.log('bisa buat KTP')` akan dijalankan.

Selain itu, kita juga bisa menggunakan boolean di kondisi. Angka 0, string kosong `""`, `null`, `undefined`, dan `NaN` semua bernilai `false`. Sedangkan selain nilai tersebut, bernilai `true`. Sebagai contoh:

```js
if (0) {
  console.log('Hello');
}
```

Kode di atas tidak akan menjalankan blok kode di dalam `if`. Lain halnya dengan

```js
if (1) {
  console.log('Hello');
}
```

Kode di atas akan menjalan blok kode di dalam `if`.

### _else_

Pernyataan `if` dapat berisi blok opsional `else` jika kondisi pada `if` bernilai _false_. Sebagai contoh:

```js
let nilai = 60;
if (nilai > 75) {
  console.log('Kamu lulus');
} else {
  console.log('Kamu tidak lulus');
}
```

Kode di atas akan menjalankan blok kode di dalam `else` karena `60 > 75` bernilai _false_.

### Pernyataan _else if_

Dalam beberapa kasus, kita ingin menguji beberapa kondisi yang berbeda-beda. Pernyataan _else if_ menjadi alternatifnya. Sebagai contoh:

```js
let nilai = 75;
if (nilai > 75) {
  console.log('Kamu lulus');
} else if (nilai < 75) {
  console.log('Kamu tidak lulus');
} else {
  console.log('Nilai kamu pas');
}
```

Kode di atas, akan menampikan `Nilai kamu pas`. Karena kondisi `75 > 75` dan `75 < 75` bernilai salah.

### Operator kondisional _?_

Dalam beberapa kasus, kita membutuhkan nilai variabel berdasarkan kondisi tertentu. Sebagai contoh:

```js
let keterangan;
let nilai = 80;
if (nilai > 75) {
  keterangan = 'lulus';
} else {
  keterangan = 'tidak lulus';
}
console.log(keterangan); // 'lulus'
```

Operator kondisional _?_ memungkinkan kita mengetik kode jadi lebih singkat dan sederhana. Operator ini biasa disebut _ternary_. Berikut gambarannya.

```js
let hasil = kondisi ? valueTrue : valueFalse;
```

Varibel akan memiliki nilai `valueTrue` jika `kondisi` bernilai `true` dan `valueFalse` jika kondisi bernilai `false`
Sebagai contoh:

```js
let nilai = 80;
let keterangan = nilai > 75 ? 'lulus' : 'tidak lulus';
console.log(keterangan); // lulus
```
