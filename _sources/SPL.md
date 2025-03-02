---
title: SPL

---

##### Sistem Persamaan Linier
Sistem Persamaan Linier (SPL) adalah kumpulan dua atau lebih persamaan linier yang memiliki variabel yang sama, dan solusi dari sistem tersebut adalah nilai variabel yang memenuhi semua persamaan secara bersamaan
##### Contoh SPL 

\begin{aligned}
    x + 2y + z &= 9 \\
    2x + y - z &= 3 \\
    3x - y + 2z &= 8
\end{aligned}


##### Metode Penyelesaian
Substitusi, eliminasi, matriks, atau eliminasi Gauss.

##### Eliminasi Gauss
Eliminasi Gauss adalah metode untuk menyelesaikan sistem persamaan linear dengan mengubahnya ke bentuk eselon baris menggunakan operasi baris elementer.
Metode ini mempermudah penyelesaian SPL dengan menghilangkan variabel secara bertahap hingga tersisa satu variabel yang bisa disubstitusi kembali.

##### Langkah-Langkah Eliminasi Gauss
1. Tulis Matriks Augmentasi
-Ubah SPL menjadi matriks augmentasi.
-Contoh:

\begin{aligned}
    x + 2y + z &= 9 \\
    2x + y - z &= 3 \\
    3x - y + 2z &= 8
\end{aligned}

*Menjadi*

\begin{bmatrix} 
1 & 2 & 1 & | 9 \\ 
2 & 1 & -1 & | 3 \\ 
3 & -1 & 2 & | 8 
\end{bmatrix}

2. Bentuk eslon Baris
-Gunakan Operasi Baris Elementer (OBE) untuk menghasilkan bentuk eselon baris:
* Elemen pivot (elemen pertama non-nol pada suatu baris) harus berada di kanan elemen pivot baris sebelumnya.
* Baris nol (jika ada) berada di bawah baris non-nol.

3. Subtitusi Balik
-Setelah matriks dalam bentuk eselon baris, lakukan substitusi balik untuk menemukan nilai variabel



    