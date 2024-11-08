# Latihan 1
```python
import random

# Meminta pengguna memasukkan nilai n
n = int(input("Masukkan nilai N: "))

# Looping untuk menghasilkan n bilangan acak
for i in range(1, n + 1):
    # Menghasilkan bilangan acak antara 1 dan 5
    bilangan_acak = random.uniform(1, 5)

    # Menampilkan data ke-i dan nilai bilangan acak
    print(f"data ke: {i} => {bilangan_acak}")
    print("Selesai")
```
# Output Latihan 1
````markdown
Masukkan nilai N: 05
data ke: 1 => 4.394507876749119
Selesai
data ke: 2 => 1.7526996875889558
Selesai
data ke: 3 => 1.761776596288391
Selesai
data ke: 4 => 3.3639255944364757
Selesai
data ke: 5 => 2.977661100071994
Selesai
````

# Penjelasan Latihan 1
Posisi "Selesai": Kata "Selesai" dicetak setelah setiap bilangan acak. Jika Anda ingin kata "Selesai" hanya dicetak setelah seluruh loop selesai, maka sebaiknya letakkan di luar loop.
Indentasi dalam loop: Indentasi dan strukturnya sudah benar, jadi Anda tidak perlu khawatir tentang itu. Berikut adalah penjelasan lengkap mengenai kode Python yang Anda berikan:
Penjelasan Langkah demi Langkah:
Import Modul random:

import random
Di bagian ini, Anda mengimpor modul random, yang memungkinkan Anda untuk menghasilkan bilangan acak. Fungsi random.uniform() digunakan untuk menghasilkan bilangan acak float dalam rentang tertentu.

Meminta Input dari Pengguna:

n = int(input("Masukkan nilai N: "))
Kode ini meminta pengguna untuk memasukkan sebuah nilai integer yang disebut n. Nilai n ini akan menentukan berapa kali loop for akan dijalankan. Fungsi input() mengambil input dari pengguna dalam bentuk string, dan kemudian fungsi int() mengubahnya menjadi tipe data integer.

Looping untuk Menghasilkan Bilangan Acak:

for i in range(1, n + 1):
Di sini, loop for akan dimulai dari i = 1 dan berjalan hingga i = n. Fungsi range(1, n + 1) menghasilkan urutan angka mulai dari 1 hingga n. Jadi, jika pengguna memasukkan n = 5, loop ini akan dijalankan 5 kali, dengan nilai i yang bervariasi dari 1 hingga 5.

Menghasilkan Bilangan Acak:

bilangan_acak = random.uniform(1, 5)
Setiap kali loop dijalankan, kode ini menghasilkan sebuah bilangan acak float di antara 1 dan 5. Fungsi random.uniform(1, 5) menghasilkan nilai acak dengan batas bawah 1 dan batas atas 5 (termasuk desimal). Hasilnya disimpan dalam variabel bilangan_acak.

Menampilkan Hasil:

print(f"data ke: {i} => {bilangan_acak}")
Di bagian ini, program menampilkan hasil bilangan acak yang telah dihasilkan. Dengan menggunakan f-string, nilai dari i (nomor urut data) dan bilangan_acak akan dicetak dalam format yang rapi, seperti "data ke: 1 => 3.12" jika nilai i adalah 1 dan bilangan_acak adalah 3.12.

Mencetak Kata "Selesai" Setiap Kali dalam Loop:

print("Selesai")
Setelah mencetak hasil untuk setiap bilangan acak, perintah ini mencetak kata "Selesai". Karena perintah ini berada di dalam loop, kata "Selesai" akan dicetak setelah setiap iterasi (setiap kali bilangan acak dicetak).

# Penjelasan Output 1
Untuk setiap iterasi dari loop:

Program mencetak bilangan acak untuk data ke-1, data ke-2, dan seterusnya.
Setelah itu, kata "Selesai"dicetak.
Kata "Selesai" akan dicetak setelah setiap bilangan acak. Jika Anda hanya ingin kata "Selesai" muncul sekali di akhir setelah seluruh loop selesai, Anda harus memindahkan print("Selesai") ke luar loop.

# Latihan 2
```python
# Inisialisasi laba per bulan
laba = 0
total_laba = 0

# Loop untuk bulan 1 sampai 8
for bulan in range(1, 9):
    # Menentukan laba berdasarkan bulan
    if bulan in [1, 2]:  # Bulan 1 dan 2
        laba = 0
    elif bulan in [3, 4]:  # Bulan 3 dan 4
        laba = 10000000.0
    elif bulan in [5, 6, 7]:  # Bulan 5, 6, dan 7
        laba = 50000000.0
    elif bulan == 8:  # Bulan 8
        laba = 200000000.0
    
    # Menampilkan laba per bulan
    print(f"laba bulan ke- {bulan} sebesar: {laba}")
    
    # Menambahkan laba ke total laba
    total_laba += laba

# Menampilkan total laba
print(f"Total laba adalah: {total_laba}")
```
# Output 2
````markdown
laba bulan ke- 1 sebesar: 0
laba bulan ke- 2 sebesar: 0
laba bulan ke- 3 sebesar: 10000000.0
laba bulan ke- 4 sebesar: 10000000.0
laba bulan ke- 5 sebesar: 50000000.0
laba bulan ke- 6 sebesar: 50000000.0
laba bulan ke- 7 sebesar: 50000000.0
laba bulan ke- 8 sebesar: 200000000.0
Total laba adalah: 370000000.0
````

# Penjelasan Kerja 1 Dan Output
Tentu, mari kita jelaskan lebih rinci program ini yang menghitung laba bulanan selama periode 8 bulan:

Inisialisasi Variabel:

python
laba = 0
total_laba = 0
Dua variabel ini diatur pada awal program. laba digunakan untuk menyimpan laba bulanan, dan total_laba digunakan untuk menghitung jumlah total laba selama 8 bulan.

Loop untuk Bulan 1 sampai 8:

python
for bulan in range(1, 9):
Baris ini mendefinisikan loop for yang akan berjalan dari bulan 1 hingga bulan 8. range(1, 9) menghasilkan urutan angka dari 1 sampai 8.

Menentukan Laba Berdasarkan Bulan:

```python
if bulan in [1, 2]:
    laba = 0
elif bulan in [3, 4]:
    laba = 10000000.0
elif bulan in [5, 6, 7]:
    laba = 50000000.0
elif bulan == 8:
    laba = 200000000.0
```
Ini adalah blok kode yang menggunakan if-elif-else untuk menentukan laba berdasarkan bulan:

Untuk bulan 1 dan 2, laba diatur menjadi 0.

Untuk bulan 3 dan 4, laba diatur menjadi Rp10.000.000.

Untuk bulan 5, 6, dan 7, laba diatur menjadi Rp50.000.000.

Untuk bulan 8, laba diatur menjadi Rp200.000.000.

Menampilkan Laba per Bulan:

```python
print(f"laba bulan ke- {bulan} sebesar: {laba}")
```
Baris ini mencetak laba untuk setiap bulan yang sedang dihitung dalam loop.

Menambahkan Laba ke Total Laba:

```python
total_laba += laba
```
Setelah laba bulanan ditentukan, nilai laba ditambahkan ke variabel total_laba untuk menghitung total laba secara keseluruhan.

Menampilkan Total Laba:

```python
print(f"Total laba adalah: {total_laba}")
```
Setelah loop selesai, baris ini mencetak total laba yang telah dihitung selama 8 bulan.

Secara keseluruhan, program ini berfungsi untuk menghitung dan menampilkan laba per bulan dan total laba setelah periode 8 bulan.

# Latihan 3 
```python
def atm():
  saldo = 10000000000

  while True:
    print("Saldo saat ini: Rp", saldo)
    print("1. Tarik Uang")
    print("2. Keluar")
    pilihan = int(input("Pilih menu (1/2): "))

    if pilihan == 1:
      jumlah_tarik = int(input("Masukkan jumlah penarikan: "))
      if jumlah_tarik <= saldo:
        saldo -= jumlah_tarik
        print("Penarikan berhasil!")
      else:
        print("Saldo tidak mencukupi!")
    elif pilihan == 2:
      print("Terima kasih telah menggunakan ATM!")
      break
    else:
      print("Pilihan tidak valid!")

atm()
```

# Output
```Markdown
Saldo saat ini: Rp 10000000000
1. Tarik Uang
2. Keluar
Pilih menu (1/2): 1
Masukkan jumlah penarikan: 500000
Penarikan berhasil!
Saldo saat ini: Rp 9999500000
1. Tarik Uang
2. Keluar
Pilih menu (1/2): 2
Terima kasih telah menggunakan ATM!
```

# Penjelasan Kerja 3 dan OutPout

Definisi Fungsi:

python
def atm():
Fungsi atm() didefinisikan untuk mengelola seluruh operasi ATM. Fungsi ini akan menjalankan proses penarikan uang dan pengecekan saldo secara berulang sampai pengguna memilih untuk keluar.

Inisialisasi Saldo:

python
saldo = 10000000000
Variabel saldo diinisialisasi dengan nilai Rp10.000.000.000 sebagai saldo awal yang tersedia di akun pengguna.

Loop Utama:

python
while True:
Loop while True digunakan untuk menjalankan proses ATM secara terus-menerus sampai pengguna memilih untuk keluar. Ini adalah loop tak terbatas yang hanya akan berhenti jika diperintahkan dengan break.

Menampilkan Menu dan Saldo:

python
print("Saldo saat ini: Rp", saldo)
print("1. Tarik Uang")
print("2. Keluar")
pilihan = int(input("Pilih menu (1/2): "))
Baris ini menampilkan saldo saat ini dan pilihan menu kepada pengguna. Pengguna diminta untuk memilih antara opsi 1 (Tarik Uang) dan opsi 2 (Keluar).

Proses Penarikan Uang:

```python
if pilihan == 1:
    jumlah_tarik = int(input("Masukkan jumlah penarikan: "))
    if jumlah_tarik <= saldo:
        saldo -= jumlah_tarik
        print("Penarikan berhasil!")
    else:
        print("Saldo tidak mencukupi!")
```
Jika pengguna memilih opsi 1, program akan meminta jumlah uang yang ingin ditarik. Jika jumlah yang diminta lebih kecil atau sama dengan saldo yang tersedia, saldo akan dikurangi dengan jumlah tersebut dan pesan sukses ditampilkan. Jika tidak, pesan kesalahan akan muncul.

Proses Keluar:

```python
elif pilihan == 2:
    print("Terima kasih telah menggunakan ATM!")
    break
```
Jika pengguna memilih opsi 2, program akan menampilkan pesan terima kasih dan menghentikan loop dengan break, yang mengakhiri fungsi atm().

Pilihan Tidak Valid:

```python
else:
    print("Pilihan tidak valid!")
```
Jika pengguna memasukkan pilihan selain 1 atau 2, program akan menampilkan pesan bahwa pilihan tidak valid.

Pemanggilan Fungsi:

```python
atm()
```
Baris terakhir dari kode ini memanggil fungsi atm() untuk memulai program ATM dan menjalankan prosesnya.

Program ini adalah simulasi sederhana dari sebuah mesin ATM yang memungkinkan pengguna untuk menarik uang dan memeriksa saldo mereka. Seluruh proses diatur dalam loop yang terus berjalan sampai pengguna memilih untuk keluar.








