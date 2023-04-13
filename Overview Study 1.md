# Mari Belajar Javascript Study 1
## Variable
### Karakteristik
Variable dapat digunakan seperti string dan integer yang sudah kita pelajari. Nilai yang diberikan ke variable dapat digabungkan dengan string lain atau digunakan dalam kalkulasi dengan integer lain.
### Update Variable
Anda dapat mengupdate nilai variable Anda. Ketika Anda menetapkan nilai baru ke variable yang telah Anda berikan nilainya, nilai baru tersebut akan menggantikan nilai yang lama. Untuk memberikan nilai baru, Anda tidak perlu menggunakan let, cukup dengan menulis variableName=nilai.

```javascript
let name = "akbar";
console.log(name);

name = "bukan akbar";
console.log(name);
```

### Update Variable Menggunakan Nilainya

Bagaimana cara menambahkan 3 ke nilai variable number yang telah dideklarasikan? Seperti gambar di bawah, Anda dapat melakukan ini dengan menetapkan number + 3 ke variable number. Dengan cara ini, hasil kalkulasi akan ditetapkan ke variable di sisi kiri.

```javascript
let number = 2;
console.log(number)

let number = number +3;
console.log(number)
```

### Penulisan Singkat
Ada shorthand untuk code seperti number = number + 10. Shorthand ini sering digunakan, jadi coba ingat format-nya sesuai contoh di bawah!
```javascript
// Penulisan Normal
x = x + 10
x = x - 10
x = x * 10
x = x / 10
x = x % 10

// Penulisan Singkat
x += 10
x -= 10
x *= 10
x /= 10
x &= 10
```
## Constant
Constant mirip dengan variable, tetapi tidak dilakukan deklarasi dengan let. Cara menentukan constant adalah dengan menggunakan kata kunci const. Lihat lebih lanjut perbedaan antara keduanya pada slide berikutnya.

```javascript
const name = "Akbar";
```

### Beda Constant dan Variable

Seperti yang dapat Anda lihat pada contoh di kiri, variable (let) dapat diperbarui. Namun, constant tidak dapat diperbarui. Jika Anda mencoba untuk memperbarui nilai constant, seperti ditunjukkan di sisi kanan, Anda akan mendapatkan pesan error.

### Manfaat Menggunakan Constant

Manfaat constant adalah untuk mencegah perubahan nilai. Sekilas mungkin terlihat tidak praktis. Namun, ini dapat mencegah perubahan yang tidak diinginkan supaya code Anda lebih aman. Semakin banyak code yang Anda tulis, semakin Anda akan merasakan manfaatnya. Untuk seterusnya, kita akan lebih sering menggunakan constant.

## Template Literal
Hingga saat ini, kita menggunakan simbol tanda tambah (+) untuk menggabungkan string dan constant. Di ES6, Anda bisa melakukan hal ini sebuah fitur yang disebut template literal. Dengan template literal, Anda dapat memasukkan constant (variable) di dalam string, seperti gambar di bawah. Mari kita lihat slide berikutnya untuk mempelajarinya lebih lanjut.
### Cara Menulis Template Literal
 Anda dapat memasukkan constant dan variable ke string dengan menulis ${someConstant}. Saat melakukan ini, Anda harus meletakkan keseluruhan string di antara dua backtick(`) . Anda juga dapat memasukkan beberapa variable dan constant seperti yang ditampilkan pada contoh di kanan.
```javascript
// Contoh 1
const name = "Ninja Ken";
console.log(`Halo ${name}`);

// Contoh 2
const name = "Ninja Ken";
const age = 14;
console.log(`${name} berusia ${age} tahun`);
```

## Percabangan Kondisional (If Else)
Selanjutnya, mari kita pelajari percabangan kondisional, sebuah konsep penting dalam pemrograman. Saat mempelajari pemrograman, akan ada saatnya di mana Anda ingin menentukan kapan code tertentu ingin dijalankan. Perintah ini disebut percabangan kondisional.
## Struktur dan pernyataan
Ketika menggunakan pernyataan if, percabangan bersyarat "jika X maka Y" akan diaktifkan. Syarat tersebut dituliskan setelah if dan code di dalam kurung kurawal { } akan dieksekusi saat syarat di dalam if terpenuhi. Pahami cara menulis pernyataan if melalui gambar di bawah ini.

```javascript

// Struktur
if (kondisi){
    // Ketik Kode Disini
}

// Contoh
const number = 12;
if(number>12){
    console.log("Number lebih besar dari 12");
}
```
## Operator Boolean dan Perbandingan
"true" yang dicetak di console pada slide sebelumnya disebut boolean. Tipe data boolean memiliki dua nilai; true dan false. Pernyataan bersyarat dinilai "true" jika syaratnya terpenuhi dan "false" jika sebaliknya. Anda dapat melihat cara kerjanya pada contoh di bawah.
```javascript
// Boolean - true
const number = 12;
console.log(number>10)

//Boolean - false
const number = 10;
console.log(number>12)

// Perbandingan Nilai
const number = 12;
console.log(number<30) // Bernilai true
const number = 12;
console.log(number<=12) // Bernilai true
const number = 12;
console.log(number>30) // Bernilai false

// Kesetaraan Nilai
const number = 12;
const name = "John";
console.log(number===12); // Bernilai true
console.log(name!=="John"); // Bernilai false

```
## Kondisi tidak terpenuhi (if else)
Ada saatnya di mana Anda harus memanggil code yang berbeda jika kondisi pernyataan if adalah false. Seperti yang ditunjukkan di bawah, Anda harus memanggil code yang berbeda untuk mencetak"Nilai kurang dari atau sama dengan 10" jika nilai angka tidak lebih besar dari 10.
```javascript
// Struktur if else
if(kondis){
    // ketika kondisi true
}else{
    // ketika kondisi false
}

// Contoh
const number = 7;
if(number>10){
    console.log("Number lebih dari 10")
}else{
    console.log("Number lebih kecil atau sama dengan 10")
}
```
## Menambahkan kondisi (else if)
Mari kita lihat cara menambahkan kondisi lebih banyak ke statement if dan else. Misalnya, kita akan mempelajari cara menambahkan pengontrolan alur untuk menyertakan kondisi yang "tidak lebih besar dari 10" tetapi "lebih besar dari 5".
```javascript
// Struktur penulisan
if(kondisi1){
    // Ketika kondisi 1 true
}else if(kondisi2){
    // Ketika kondisi 1 false dan kondisi 2 true
}else{
    // Ketika tidak ada kondisi yang true
}
// Contoh
const number = 7;
if(number>10){
    console.log("number lebih besar dari 10"); //Bernilai false
}else if(number>5){
    console.log("number lebih besar dari 5"); //Bernilai true
}else{
    console.log("number lebih kecil atau sama dengan 5");
}
```
## Persyaratan && (Dan)
Selanjutnya kita akan pelajari cara menggabungkan beberapa syarat. Pertama, kita akan mempelajari &&. Syarat 1 && Syarat 2 berarti "Syarat 1 dan Syarat 2" di mana hanya jika semua persyaratan bernilai true, maka keseluruhan ekspresi bernilai true. Contohnya "Lebih besar dari 10 dan lebih kecil dari 30" tidak dapat ditulis sebagai 10 < x < 30. Pada kasus ini, gunakan &&!
## Persyaratan || (atau)
Selanjutnya, kita akan mempelajari simbol yang berarti "OR" (Atau). Atau diekspresikan dalam bentuk ||. Syarat 1 || Syarat 2 berarti "Syarat 1 atau Syarat 2". Pada kasus ini, di antara beberapa syarat, jika salah satunya bernilai true, maka keseluruhan ekspresi menjadi true.
```javascript
// Contoh DAN
const number = 31;
if (number >=10 && number < 100){
    console.log("Number berdigit 2");
}

// Contoh ATAU
const name = "Andi";
if (name === "Budi" || name === "Andi"){
    console.log("Anak Sekolah XYZ");
}
```
## Pernyataan Switch
Cara lain untuk menggunakan alur kontrol, adalah pernyataan switch. Gambar di bawah adalah contoh untuk mendasarkan alur pengontrolan pada nilai constant warna yang menyimpan warna lampu lalu lintas. Anda akan dapat menggunakan pernyataan switch ketika percabangan code tergantung pada nilai tertentu. Lihat slide berikutnya untuk informasi lebih detail!
```javascript
// Struktur penulisan
switch(nilai kondisional){
    // Perintah untuk memilih salah satu switch
    case nilai1:
        // Hasil perintah
        break;
    case nilai2:
        // Hasil perintah
        break;
    // dan seterusnya
}

// Contoh
const color = "merah";
switch(color){
    // Perintah untuk memilih salah satu switch
    case "merah":
        console.log("Berhenti!");
        break;
    case "hijau":
        console.log("Jalan");
        break;
    case "kuning":
        console.log("Hati-Hati");
        break;
}
```
## Pernyataan Switch - Default
Seperti yang telah Anda pelajari, jika nilai kondisi switch cocok dengan nilai untuk kasus tertentu, bagian code itu akan berjalan. Namun, jika nilai tidak cocok dengan kondisi apa pun, case default akan dipanggil. Default mirip dengan else yang digunakan untuk statement if.
```javascript
// Struktur penulisan
switch(nilai kondisional){
    // Perintah untuk memilih salah satu switch
    case nilai1:
        // Hasil perintah
        break;
    case nilai2:
        // Hasil perintah;
        break;
    default:
        // Hasil Perintah;
        break;
}

// Contoh
const color = "merah";
switch(color){
    // Perintah untuk memilih salah satu switch
    case "merah":
        console.log("Berhenti!");
        break;
    case "hijau":
        console.log("Jalan");
        break;
    case "kuning":
        console.log("Hati-Hati");
        break;
    default:
        console.log("Nilai color salah");
        break;
}
```
