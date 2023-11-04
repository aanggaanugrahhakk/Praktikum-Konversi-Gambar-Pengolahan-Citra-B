
# Konversi Gambar

Konversi gambar adalah salah satu tahap dalam pengolahan citra yang bertujuan untuk mengubah format gambar dari satu bentuk ke bentuk lainnya.

Library yang digunakan:

- cv2: OpenCV (Open Source Computer Vision) adalah pustaka fungsi pemrograman yang terutama ditujukan untuk visi komputer waktu nyata. Library ini menyediakan berbagai macam fungsi untuk pemrosesan gambar dan video, termasuk pemfilteran gambar, deteksi fitur, pengenalan objek, dan banyak lagi. Perpustakaan cv2 adalah pembungkus Python untuk perpustakaan OpenCV, yang memungkinkan pengembang untuk menggunakan fungsi OpenCV dalam kode Python.
- NumPy: NumPy adalah library Python yang digunakan untuk bekerja dengan larik. NumPy menyediakan objek larik N-dimensi yang kuat, serta fungsi-fungsi untuk bekerja dengan larik ini. NumPy sering digunakan dalam pemrosesan gambar dan aplikasi visi komputer untuk tugas-tugas seperti pemfilteran gambar, ekstraksi fitur, dan banyak lagi.

Penjelasan penyelesaian Konversi Gambar yang digunakan di skrip:

- Skrip yang diberikan ditulis dalam bahasa Python dan menggunakan Library OpenCV (cv2) dan NumPy untuk pemrosesan gambar. Skrip tersebut membaca file gambar bernama 'citra_medis.jpg' dan menampilkannya menggunakan fungsi cv.imshow(). Skrip kemudian mencetak bentuk dan tipe data gambar menggunakan atribut .shape dan .dtype dari array gambar.
- Skrip kemudian mengekstrak saluran biru, hijau, dan merah dari gambar menggunakan pemotongan array dan menetapkannya ke variabel b, g, dan r, masing-masing. Skrip kemudian membuat gambar grayscale baru dengan mengulang setiap piksel dari gambar asli dan menghitung jumlah tertimbang dari nilai merah, hijau, dan biru menggunakan rumus: 0.2989 * r + 0.587 * g + 0.1141 * b. Gambar abu-abu yang dihasilkan disimpan dalam array NumPy baru yang disebut medical_gray dan ditampilkan menggunakan cv.imshow().
- Skrip kemudian mengubah citra grayscale menjadi citra biner dengan mengulang setiap piksel dari citra grayscale dan mengatur piksel yang sesuai dalam array NumPy baru yang disebut medical_biner menjadi 1 jika nilai piksel kurang dari nilai ambang batas 255, dan 0 jika tidak. Gambar biner yang dihasilkan ditampilkan menggunakan cv.imshow().
- Terakhir, skrip mencetak nilai piksel dari gambar grayscale dan biner pada posisi (50,50) menggunakan operator pengindeksan [].

Berikut alur penjelasan skrip tersebut:

- Membaca file gambar bernama 'citra_medis.jpg' menggunakan fungsi cv.imread() dan menampilkannya menggunakan fungsi cv.imshow().
- Mencetak bentuk dan tipe data gambar menggunakan atribut .shape dan .dtype dari array gambar.
- Mengekstrak saluran biru, hijau, dan merah dari gambar menggunakan pemotongan array dan menetapkannya ke variabel b, g, dan r.
- Membuat gambar grayscale baru dengan mengulang setiap piksel dari gambar asli dan menghitung jumlah tertimbang dari nilai merah, hijau, dan biru menggunakan rumus: 0.2989 * r + 0.587 * g + 0.1141 * b. Gambar abu-abu yang dihasilkan disimpan dalam array NumPy baru yang disebut medical_gray dan ditampilkan menggunakan cv.imshow().
- Mengubah gambar grayscale menjadi gambar biner dengan mengulang setiap piksel gambar grayscale dan mengatur piksel yang sesuai dalam array NumPy baru yang disebut medical_biner menjadi 1 jika nilai piksel kurang dari nilai ambang batas 255, dan 0 jika tidak. Gambar biner yang dihasilkan ditampilkan menggunakan cv.imshow().
- Mencetak nilai piksel dari gambar grayscale dan biner pada posisi (50,50) menggunakan operator pengindeksan [].

Sitasi:
- [1] https://www.semanticscholar.org/paper/00442d8951be90f8c312495271abcf3ff2f3a131
- [2] https://www.semanticscholar.org/paper/bd9285c7411ee3fcdf1d1fc16e6139d3d4e32c4f
- [3] https://www.semanticscholar.org/paper/839e591c068b99903cb9a409db78135093b58f50
- [4] https://www.semanticscholar.org/paper/bc647bce9dbfe73867d40a07b680827435d8e256
- [5] https://www.semanticscholar.org/paper/beb882d5c2821f167b34189e0af1f07eecb62991
- [6] https://www.semanticscholar.org/paper/e7c7a170ba86a6edd36961a6560d92876ff1d5dc
- [7] https://www.semanticscholar.org/paper/d987cb2d5135bf589cffcb02e30877bb075700b3
- [8] https://www.semanticscholar.org/paper/495d5da29240c2b3facc7bd0bedbd9c40f34f113
- [9] https://www.semanticscholar.org/paper/839e591c068b99903cb9a409db78135093b58f50
- [10] https://www.semanticscholar.org/paper/09457e0b3d187097bd986224481d8204890d01ac
- [11] https://www.semanticscholar.org/paper/beb882d5c2821f167b34189e0af1f07eecb62991
- [12] https://www.semanticscholar.org/paper/9bff4e5cb0fd552306b025226e5f493f236071c7
- [13] https://www.semanticscholar.org/paper/beb882d5c2821f167b34189e0af1f07eecb62991
- [14] https://www.semanticscholar.org/paper/d987cb2d5135bf589cffcb02e30877bb075700b3
- [15] https://www.semanticscholar.org/paper/bc647bce9dbfe73867d40a07b680827435d8e256
- [16] https://www.semanticscholar.org/paper/839e591c068b99903cb9a409db78135093b58f50
- [17] https://www.semanticscholar.org/paper/00442d8951be90f8c312495271abcf3ff2f3a131
- [18] https://www.semanticscholar.org/paper/b2f730969733aadd91e89d3d34bb2c2c59d632bd
- [19] https://www.semanticscholar.org/paper/d987cb2d5135bf589cffcb02e30877bb075700b3
- [20] https://www.semanticscholar.org/paper/beb882d5c2821f167b34189e0af1f07eecb62991
- [21] https://www.semanticscholar.org/paper/bc647bce9dbfe73867d40a07b680827435d8e256
- [22] https://www.semanticscholar.org/paper/839e591c068b99903cb9a409db78135093b58f50
- [23] https://www.semanticscholar.org/paper/e532205af0ba47063cca10d5571c64503068f9d0
- [24] https://www.semanticscholar.org/paper/00442d8951be90f8c312495271abcf3ff2f3a131
- [25] https://www.perplexity.ai/search/Konversi-Gambar-di-Gj4rUCSSQXaPl1QtSE5lGQ?s=c
## 🔗 Link Data Diri
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/anugrahak)

## Authors

- Anugrah AK. [@aanggaanugrahhakk](https://www.github.com/aanggaanugrahhakk)


## Identitas Authors

Nama: Anugrah AK.

NIM: 202131037

Kelas: B
