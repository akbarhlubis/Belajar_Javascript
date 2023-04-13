# Mari Belajar Javascript Study 2
## Loop While
Salah satu cara melakukan iterasi adalah dengan menggunakan loop while. Loop ini ditulis seperti yang ditampilkan dalam contoh di gambar bawah. "Selama syaratnya bernilai true", code di dalam tanda kurung kurawal {} akan diulang. Anda tidak perlu menempatkan titik koma diakhir code loop while.
```javascript
// Struktur
while(kondisi){
    // Hasil code
    // diakhiri dengan FALSE agar tidak terjadi looping infinity
}

// Contoh
let number = 1;
while (number <= 10){
    console.log(number);
    number+=1;
}
```
## Loop For
Ada cara lain untuk melakukan iterasi: loop for. Meskipun pada dasarnya memberikan hasil yang sama, loop for dapat ditulis dalam bentuk yang lebih sederhana dibandingkan loop while.
Mari kita pelajari secara lebih terperinci dalam slide berikut ini.
```javascript
// Struktur
for(variable;kondisi;update){
    // Penulisan kode
}

// Contoh
for(let number = 1;number<=100;number+=1){
    console.log(number);
}

// Penyingkatan agar lebih efektif
for(let number = 1;number<=100;number ++){
    console.log(number);
}
```
## Menangani banyak nilai (Array)
Mari kita pelajari cara menangani beberapa nilai.
Misalnya, bila terdapat nama buah-buahan yang berbeda sebagai nilai, membuat istilah seperti "daftar buah" akan lebih mudah dibandingkan mendefinisikannya sebagai variable yang terpisah. 
```javascript
// Struktur
nilai = [nilai1, nilai2, nilai3]
kalimat = ["kalimat1","kalimat2","kalimat3"]

// contoh
let animals = ["anjing","kucing","domba"]
console.log(animals)

// Nomor index, dimulai dari nilai pertama adalah 0
let animals = ["anjing","kucing","domba"]
console.log(animals[0])

// mengupdate nilai
let animals = ["anjing","kucing","domba"]
console.log(animals[0])
animals[0 = "komodo"]
console.log(animals[0])

// Iterai dengan array
const animals = ["anjing", "kucing", "domba"];

for (let i = 0; i <3;i++) {
    console.log(animals[i])
    
}

// Property length
const animals = ["anjing", "kucing", "domba"];

for (let i = 0; i <animals.length;i++) {
    console.log(animals[i])
    
}
```
## Object dan Array
Object, seperti array, digunakan untuk mengelompokkan dan mengelola beberapa nilai. Bila array mengatur nilai secara berurutan berdasarkan index, objects mengelola nilai dengan memberikannya nama yang disebut property.
```javascript
// Struktur
{property1:nilai1,property2:nilai2};

// Contoh
const manusia = {nama:"akbar",beratBadan:60};
console.log(manusia);

// Mendapatkan nilai object
const manusia = {nama:"akbar",beratBadan:60};
console.log(manusia.nama);

// Update nilai Object
const manusia = {nama:"akbar",beratBadan:60};
console.log(manusia);
manusia.nama="bukanAkbar"
console.log(manusia.nama);

// Object yang memiliki array
const manusia = [
    {nama:"akbar",usia:20},
    {nama:"human",usia:10000}
];
console.log(manusia);
console.log(manusia[0]);
console.log(manusia[0].usia);

// Array dan Iterasi
const characters = [
    {name: "Ninja Ken", age: 14},
    {name: "Guru Domba", age: 100},
    {name: "Baby Ninja Ben", age: 5},
  ];
  
  // Selesaikan loop for di bawah
  for (let i=0;i<characters.length ;i++) {
    console.log("--------------------");
    
    // Tentukan nilai constant character
    const character = characters[i];
    
    // Cetak "Nama saya adalah ____"
    console.log(`Nama saya adalah ${character.name}`);
    
    // Cetak "Saya berusia ____ tahun"
    console.log(`Saya berusia ${character.age} tahun`);
    
  }

  
```
