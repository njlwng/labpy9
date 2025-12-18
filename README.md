# LATIHAN PRAKTIKUM 9

Nama : Najla Wening Khairunnisa

Nim : 312510225

Kelas : TI.25.A2

Mata Kuliah : Pengantar Pemrograman

## Materi

Python String (Pertemuan 14)

---

## Tujuan Praktikum

Tujuan dari praktikum ini adalah untuk memahami konsep dasar string pada bahasa pemrograman Python. Mahasiswa diharapkan mampu melakukan berbagai operasi string, menggunakan format string, serta menerapkan konsep string dalam studi kasus sederhana berupa validasi data input.

---

## Dasar Teori

String merupakan tipe data yang digunakan untuk menyimpan data berupa teks. Dalam Python, string dapat dibuat dengan menggunakan tanda petik satu (') atau tanda petik dua ("). Python menyediakan berbagai fungsi bawaan untuk memanipulasi string, seperti menghitung panjang string, mengambil karakter tertentu, mengubah bentuk huruf, serta melakukan pengecekan isi string.

---

## Langkah Percobaan dan Pembahasan

### A. Latihan 1 – Operasi String

**Kode Program:**

```python
txt = "Hello World"

print(len(txt))
print(txt[-1])
print(txt[2:5])
print(txt.replace(" ", ""))
print(txt.upper())
print(txt.lower())
print(txt.replace("H", "J"))
```

**Pembahasan:**
Latihan ini menunjukkan berbagai operasi dasar string seperti menghitung jumlah karakter, mengambil karakter tertentu berdasarkan indeks, menghilangkan spasi, mengubah huruf menjadi besar dan kecil, serta mengganti karakter dalam sebuah string.

**Kesimpulan Latihan 1:**
Dari latihan ini dapat disimpulkan bahwa Python menyediakan fungsi bawaan yang memudahkan dalam pengolahan data bertipe string.

---

### B. Latihan 2 – String Format

**Kode Program:**

```python
umur = 24
txt = 'Hello, nama saya john, dan umur saya adalah {} tahun'

print(txt.format(umur))
```

**Pembahasan:**
Latihan ini membahas penggunaan metode `format()` untuk menyisipkan nilai ke dalam string. Dengan metode ini, penggabungan data menjadi lebih rapi dan mudah dibaca.

**Kesimpulan Latihan 2:**
Penggunaan format string memudahkan pembuatan teks yang bersifat dinamis tanpa perlu menggabungkan string secara manual.

---

### C. Studi Kasus – Validasi Form Input

**Kode Program:**

```python
nama = input("Masukkan nama lengkap: ")
telepon = input("Masukkan nomor telepon: ")
email = input("Masukkan email: ")

valid = True

if not nama.replace(" ", "").isalpha():
    print("Error: Nama harus hanya berisi huruf")
    valid = False

if not telepon.isdigit():
    print("Error: Nomor telepon harus hanya berisi angka")
    valid = False

if "@" not in email or "." not in email:
    print("Error: Email tidak valid")
    valid = False

if valid:
    print("Data pendaftaran valid")
```

**Pembahasan:**
Pada studi kasus ini, operasi string digunakan untuk memvalidasi data input pengguna. Pengecekan dilakukan agar data yang dimasukkan sesuai dengan ketentuan yang telah ditetapkan.

**Kesimpulan Studi Kasus:**
Operasi string dapat digunakan untuk membantu memastikan kevalidan data input sehingga kesalahan dapat diminimalkan sejak awal.

---

## Kesimpulan Akhir

Berdasarkan hasil praktikum yang telah dilakukan, dapat disimpulkan bahwa string merupakan tipe data yang sangat penting dalam Python. Dengan memanfaatkan fungsi-fungsi bawaan string, pengolahan teks dan validasi data dapat dilakukan dengan mudah dan efektif.

---

## Penutup

Demikian laporan praktikum Python String ini dibuat sebagai bentuk pemahaman terhadap materi yang telah dipelajari. Diharapkan praktikum ini dapat menjadi dasar dalam pengembangan program Python yang lebih kompleks ke depannya.



