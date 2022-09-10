## Tipe Data

Dalam bahasa pemrograman JavaScript terdapat beberapa tipe data yang dapat digunakan, seperti _string_ atau _boolean_.
<br>
JavaScript mendukung _dynamcally typed_ yang artinya terdapat tipe data yang variabelnya tidak terikat dengan tipe data lainnya. Contoh:

```js
let pesan = 'Hello World';
pesan = true;
```

Pada kasus di atas, variabel `pesan` akan memberikan nilai `true` dengan tipe data `boolean`.

### Number

```js
let x = 3456;
x = 34.34;
```

Tipe data `number` merepresentasikan nilai berbentuk angka, baik bilangan bulat maupun bilangan desimal yang keduanya disebut dengan nilai numerik reguler. Selain nilai numerik reguler, terdapat juga "nilai numerik spesial" yaitu `Infinity`, `-Infinity`, dan `NaN`.

- `Infinity` mewakili nilai matematis ∞.

```js
console.log(1 / 0); // Infinity
```

- `NaN` mewakili error yang merupakan hasil operasi matematika yang salah atau tak terdefinisi.

```js
console.log('hello world' / 2); // NaN,
```

### String

Tipe data _string_ harus diapit dengan tanda petik. Ada 3 tipe tanda petik yang dapat digunakan di JavaScript, yaitu:

- Petik ganda: `"Hello"`
- Petik tunggal: `'Hello'`
- Backtik: `` `Hello` ``

```
let nama = "Budi";
let alamat = 'Bandung';
let greet = `Hello ${nama}`;
console.log(nama); // output: Budi
console.log(alamat); // output: Bandung
console.log(greet); // output: Hello Budi
```

### Boolean

Tipe data boolean hanya memiliki dua nilai yaitu `true` dan `false`. Sebagai contoh

```js
let pesanTerkirim = true; // ya, pesan terkirim
let uangTerkirim = false; // tidak, uang tidak terkirim.
```

Nilai boolean juga dapat dihasilkan dari perbandingan 2 variabel.

```js
let lebihKecil = 2 > 1;
console.log(lebihKecil); // output menghasilkan true
let strSama = 'Hello' == 'hello';
console.log(strSama); // output menghasilkan false
```

### Nilai _null_

Nilai `null` bersifat spesial, ia bukan bagian dari tipe data yang telah dijelaskan sebelumnya.

```js
let nama = null;
```

Dalam JavaScript, `null` tidak merefensi ke objek yang tak ada, hampa, atau kosong.

### Nilai _undefined_

Nilai `undefined` juga bersifat spesial tetapi berbeda dengan `null`. Ia memiliki arti "nilai yang tidak ditetapkan" yang disebabkan sebuah variabel dideklarasikan tetapi nilainya tidak ditetapkan atau variabel dideklarasikan dengan nilai `undefined`. Sebagai contoh:

```js
let nama;
console.log(name); // output: undefined

let umur = undefined;
console.log(umur); // output: undefined
```

Penggunaan `undefined` tidak disarankan, tetapi lebih baik menggunakan `null`. Kita dapat menggunakan `undefined` untuk pengecekan apakah sebuah nilai dari variabel yang telah ditetapkan.
