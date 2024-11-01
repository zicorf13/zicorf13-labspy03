# PRAKTIKUM 4

# NAMA : ZICO RIZKY FEBRIAN

# KELAS : IE.23 C.12

# NIM : 352310880

# PENJELASAN :

# ![latihan 1](https://github.com/user-attachments/assets/6b9d5854-56e2-4cef-997d-5ace542b5d77)


Import Library:

Mengimpor modul random untuk menggunakan fungsi random() yang menghasilkan bilangan acak antara 0 dan 1.
Input dari Pengguna:

Program meminta pengguna untuk memasukkan nilai n, yaitu jumlah bilangan acak yang akan dihasilkan. Nilai ini disimpan dalam variabel n.
Inisialisasi Counter:

Inisialisasi variabel count dengan nilai 1. Variabel count ini digunakan sebagai penghitung jumlah bilangan acak yang telah dihasilkan yang memenuhi syarat (yaitu kurang dari 0.5).
Looping dengan Kondisi While:

Program menggunakan loop while dengan kondisi count <= n, yang berarti loop akan terus berjalan selama count belum mencapai nilai n.
Langkah-langkah dalam Loop:
Menghasilkan bilangan acak baru menggunakan random.random(), yang disimpan dalam variabel rand_num.
Memeriksa apakah rand_num kurang dari 0.5:
Jika ya, bilangan tersebut dicetak bersama nomor urutnya (data ke-count), dan variabel count ditambah 1.
Jika tidak, program akan menghasilkan bilangan acak baru tanpa menambah nilai count.
Mengakhiri Program:

Setelah count mencapai nilai n, loop while akan berhenti.
Program mencetak pesan "Selesai" untuk menandakan bahwa proses telah selesai.
Ringkasan Alur
Mulai: Input nilai n
Inisialisasi: count = 1
Loop:
Generate bilangan acak rand_num
Jika rand_num < 0.5:
Cetak rand_num
Tambah count
Ulangi sampai count > n
Selesai: Cetak "Selesai"
Dengan algoritma ini, program akan menghasilkan n bilangan acak yang semuanya kurang dari 0.5 dan menampilkannya satu per satu.

Inisialisasi:

Buat variabel terbesar dan set nilainya ke None. Variabel ini akan digunakan untuk menyimpan bilangan terbesar yang ditemukan selama proses input.
Loop untuk Input:

Lakukan while True untuk membuat loop yang akan terus berjalan hingga pengguna memasukkan 0.
Input Bilangan:

Di dalam loop, minta pengguna memasukkan bilangan. Setiap bilangan yang dimasukkan akan disimpan dalam variabel bilangan.
Cek Kondisi Berhenti:

Jika bilangan bernilai 0, hentikan loop menggunakan break. Ini menandakan bahwa pengguna sudah selesai memasukkan bilangan.
Cek Bilangan Terbesar:

Jika terbesar masih None (berarti ini adalah bilangan pertama yang dimasukkan) atau bilangan yang baru dimasukkan lebih besar dari terbesar:
Update nilai terbesar dengan bilangan yang baru dimasukkan.
Dengan cara ini, terbesar akan selalu menyimpan nilai bilangan yang paling besar sejauh ini.
Tampilkan Hasil:

Setelah keluar dari loop, periksa apakah ada bilangan yang telah dimasukkan.
Jika terbesar bukan None, cetak bilangan terbesar yang ditemukan.
Jika terbesar masih None, artinya pengguna tidak memasukkan bilangan sama sekali (langsung memasukkan 0), maka tampilkan pesan "Tidak ada bilangan yang dimasukkan."
Contoh Alur Eksekusi
Misalkan pengguna memasukkan bilangan secara berurutan: 10, 30, 100, 3, 20, 30, 50, lalu 0 untuk berhenti.

Iterasi 1: bilangan = 10, terbesar di-update ke 10.
Iterasi 2: bilangan = 30, terbesar di-update ke 30.
Iterasi 3: bilangan = 100, terbesar di-update ke 100.
Iterasi 4: bilangan = 3, terbesar tetap 100 (tidak berubah).
Iterasi 5: bilangan = 20, terbesar tetap 100.
Iterasi 6: bilangan = 30, terbesar tetap 100.
Iterasi 7: bilangan = 50, terbesar tetap 100.
Iterasi 8: bilangan = 0, loop berhenti.
Setelah keluar dari loop, program mencetak "Bilangan terbesar adalah: 100".

Ringkasan
Alur ini secara efektif memastikan bahwa:

Program menerima sejumlah input bilangan.
Menyimpan bilangan terbesar yang ditemukan selama input.
Menghentikan proses jika 0 dimasukkan dan menampilkan hasil bilangan terbesar.
Inisialisasi Variabel

investasi_awal diatur dengan nilai 100 juta (100.000.000), ini adalah modal awal yang diinvestasikan.
total_laba diatur dengan nilai 0 untuk menampung akumulasi laba dari bulan ke bulan.
laba_bulanan diatur dengan nilai 0, yang akan digunakan untuk menyimpan laba setiap bulan.
Looping untuk Setiap Bulan

Program menggunakan perulangan for dengan rentang 1 hingga 8, yang merepresentasikan setiap bulan dari bulan 1 sampai bulan 8.
Di setiap iterasi, program akan mengecek bulan keberapa saat ini, lalu menghitung laba bulanan sesuai dengan kondisi yang ditentukan.
Kondisi Laba Berdasarkan Bulan

Bulan 1 dan 2:
Pada dua bulan pertama, laba bulanan adalah 0 karena belum ada keuntungan, sehingga laba_bulanan tetap 0.
Bulan 3:
Mulai mendapatkan laba sebesar 1% dari investasi_awal. Jadi, laba_bulanan = investasi_awal * 0.01.
Bulan 5:
Laba meningkat menjadi 5% dari investasi_awal. Maka, laba_bulanan = investasi_awal * 0.05.
Bulan 8:
Laba menurun sebesar 2%, sehingga laba menjadi 3% dari investasi_awal. Maka, laba_bulanan = investasi_awal * 0.03.
Bulan Lainnya (Default):
Pada bulan selain yang disebutkan di atas (misalnya, bulan ke-4, ke-6, dan ke-7), laba tetap 1% dari investasi_awal. Jadi, laba_bulanan = investasi_awal * 0.01.
Penambahan Laba ke Total Laba

Setiap bulan, laba bulanan (laba_bulanan) ditambahkan ke total_laba untuk mengakumulasi total laba selama 8 bulan.
Menampilkan Laba Bulanan

Setelah menghitung laba untuk bulan tertentu, program menampilkan laba tersebut menggunakan print(f"Laba bulan ke-{bulan} sebesar: {int(laba_bulanan)}").
Menampilkan Total Laba

Setelah loop selesai, total laba yang sudah dikumpulkan selama 8 bulan akan ditampilkan dengan print(f"Total laba adalah: {int(total_laba)}").
Contoh Output
Output program akan menampilkan laba setiap bulan dan total laba setelah 8 bulan, sesuai contoh dalam screenshot tugas.

Ringkasan
Program ini menghitung laba berdasarkan persentase yang berubah-ubah tiap bulan.
Dengan kondisi bulan ke-3, ke-5, dan ke-8 yang memiliki persentase laba khusus, program mengakumulasi laba dari semua bulan ke dalam total_laba.
Pada akhirnya, program menampilkan total laba setelah 8 bulan usaha berjalan.
