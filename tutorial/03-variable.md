## Variable

Variabel adalah tempat untuk menampung data. Pada umumnya, variabel di JavaScript menggunakan `let`. Di bawah ini contoh pendeklarasian variabel _name_

```js
let name;
```

Kemudian, kita bisa memberi data ke dalam variabel _name_ dengan menggunakan operator tetap `=`.

```js
let name;
name = 'Budi';
console.log(`Hello ${name}`); // Hello Budi
```

Agar penulisan ringkas, kita bisa meringkasnya dalam satu baris dan juga

```js
let name = 'Budi';
console.log(`Hello ${name}`); // Hello Budi
```

_Note: Mendeklarasikan variabel yang sama sebanyak dua kali atau lebih akan menciptakan error._

```js
let name = 'Budi';
let name = 'Wawan';
```

Kasus di atas, akan menghasilkan pesan error. Berbeda dengan kasus berikut

```js
let name = 'Budi';
name = 'Wawan';
```

ia akan menghasilkan nilai dari variabel `name` adalah `Wawan`.

### Penamaan Variabel

Dalam penamaan variabel di JavaScript, hanya ada dua aturan, yaitu:

- Nama hanya boleh terdiri dari huruf, angka, atau simbol `$` atau `_`.
- Karakter pertama tidak diperbolehkan dalam bentuk angka.

Sebagai bentuk valid:

```js
let userAddress;
let userId12;
```

Simbol `$` dan `_` juga bisa digunakan dalam nama variabel. Sebagai contoh:

```js
let $ = 'Budi';
let _ = 'Wawan';
console.log($ + _); // BudiWawan
```

Berdasarkan beberapa aturan tersebut, akan ditunjukkan juga penamaan variabel yang tidak valid:

```js
let 1name;
let first-name;
```

## Konstan

Seperti halnya `let`, `const` juga bisa digunakan dalam mendeklarasikan sebuah variabel, tetapi `const` memilki nilai yang tidak bisa berubah. Sebagai contoh:

```js
const name = 'Budi';
```

Berbeda halnya jika kita memperlakukannya seperti `let`, ia akan menghasilkan error.

```js
const name = 'Budi';
name = 'Wawan';
```

Kasus di atas akan error, karena variabel `name` memiliki nilai `Budi`.

## Var

Pendeklarasian variabel dengan `var` dan `let` bersifat sama. Namun, `var` biasanya tidak digunakan di dalam skrip modern. Perbedaan antara `var` dan `let` penting untuk dipelajari. Berikut kasus perbedaan keduanya:

```js
if (true) {
  var name = 'Budi';
}
console.log(name); // Budi
```

Karena `var` mengabaikan blok kode, maka `var` merupakan global variabel.
Sedangkan jika menggunakan `let`, maka variabel hanya dapat diakses di dalam blok `if` saja. Sebagai contoh:

```js
if (true) {
  let name = 'Budi';
  console.log(name); // Budi
}
console.log(name); // Error: name is not defined
```

_Note: Variabel `var` bisa dideklarasikan ulang_

```js
var name = 'Wawan';
var name = 'Budi';
console.log(name); // Budi
```
