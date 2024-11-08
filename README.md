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

Penjelasan Output
Untuk setiap iterasi dari loop:

Program mencetak bilangan acak untuk data ke-1, data ke-2, dan seterusnya.
Setelah itu, kata "Selesai"dicetak.
Kata "Selesai" akan dicetak setelah setiap bilangan acak. Jika Anda hanya ingin kata "Selesai" muncul sekali di akhir setelah seluruh loop selesai, Anda harus memindahkan print("Selesai") ke luar loop.
# Penjelasan Outpu 1
Untuk setiap iterasi dari loop:

Program mencetak bilangan acak untuk data ke-1, data ke-2, dan seterusnya.
Setelah itu, kata "Selesai"dicetak.
Kata "Selesai" akan dicetak setelah setiap bilangan acak. Jika Anda hanya ingin kata "Selesai" muncul sekali di akhir setelah seluruh loop selesai, Anda harus memindahkan print("Selesai") ke luar loop.
