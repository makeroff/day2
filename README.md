# Rangkuman Hari Kedua

Di hari kedua bootcamp **Refactory** kita mulai di ajarkan tentang dasar-dasar javascript, banyak sekali yang di pelajari mulai dari *variable, method, function, array dan object*.


## Variable Javascript.
Ada 3 cara mendeklarasikan variabel pada javascript yang memiliki perbedaan masing-masing.

- **var** = bisa di asign ulang - redefinisi

- **let** = bisa berubah  / dinamis


- **const** = mendeklarasikan sebuah variable yang bernilai statis, dan tidak bisa di ubah

## JavaScript String

- **split()** perintah untuh memisahkan string berdasarkan value yang kita masukkan
- **join()** perintah untuk menggabungkan array berdasarkan value yang kita masukkan
- **toLowerCase()** = merubah semua menjadi huruf kecil
- **toUpperCase()** = merubah semua menjadi huruf besar

- **charAt(0)** = memilih charakter pada index 0

- **splice()** = perintah untuk memotong string

## Mendeklarasikan String
```javascript
var a = 'halo ganteng'
let b = 'Aku juga ganteng'
const c = new String('Aku aja yang ganteng, kamu enggak')

```

<br>

### Mengubah String menjadi Array
```javascript
let text = 'Pagi pagi belajar javascript'
splitted = text.split(' ')
console.log(splitted)
```

### Mengubah huruf besar di awal kalimat

```javascript
function capitalize(string){
    let arr = string.split(' ')
    for(let i = 0; i < arr.length; i++){
        arr[i] = arr[i].charAt(0).toUpperCase() + arr[i].slice(1)
    }
    let result = arr.join(' ')
    console.log(result)
}
```

### Mengubah Array ke String
```javascript
const want = ['Saya', 'ingin', 'makan', 'Jeruk'];
const print = want.join(' ');
console.log(print);

```

## Object
**Object** adalah sebuah variabel yang menyimpan key dan value.

### Cara pelulisan object
```javascript 
const a = {}
const b = new Object()
const c = {a : 'kamu lagi apa', b : 'aku lagi belajar'}

```

### Mengakses nilai dari object
```javascript
const beli = { buah: 'Mangga', harga: '1000'}
// Mengakses buah
console.log(beli.buah)// output Mangga
// Mengakses harga
console.log(beli.harga)// output: 1000
```


## Array
**Array** merupakan struktur data yang digunakan untuk menyimpan sekumpulan data dalam satu tempat. Setiap data dalam **Array** memiliki indeks, sehingga kita akan mudah memprosesnya.

### Cara membuat array
```javascript
const tahun = [2001, 2002, 2005]
const kota = ['malang', 'surabaya', 'jakarta', 'medan']
const buah = new Array('Melon', 'Anggur', 'Semangka')

```

### Cara Mengakses Array
```javascript
const tahun = [2001, 2002, 2005]
const kota = ['malang', 'surabaya', 'jakarta', 'medan']
const buah = new Array('Melon', 'Anggur', 'Semangka')

// Memanggil array pada index 0
console.log(tahun[0])// Output: 2001
```

### Array Methods
1. **Array.push()** menambahkan item pada array ke index terakhir

2. **Array.pop()** menghapus item pada index terakhir

3. **Array.shift** menghapus item pada index pertama

4. **Array.unshift()** menambahkan item pada index pertama

5. **Array.concat()** menyambung array / menggabungkan array

6. **Array.sort()** mengurutkan array berdasarkan alpabet / angka

7. **Array.reverse()** membalik urutan array

### Mengakses Array

```javascript
const purchases = [
    { items: ['Pisang', 'Apel'], total: 1000, onSale: false},
    { items: ['Nanas', 'Anggur'], total: 3000, onSale: false},
    { items: ['Melon', 'Semangka'], total: 5000, onSale: true},
    { items: ['Pisang', 'Jeruk'], total: 5200, onSale: false}
]

// memanggil  index ke 3 key total
result = purchases[3].total;
console.log(result); // out 5200

// memanggil  index ke 3 key item index ke 0
result = purchases[3].items[0];

console.log(result);// out Pisang
```