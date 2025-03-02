---
title: SPL PENYELESAIAN 3 PERSAMAAN

---

##### SPL 3 VARIABEL
###### Sistem Persamaannya : 
\begin{aligned}
    x + y + z &= 6 \\
    2x - y + 3z &= 14 \\
    3x + 4y + z &= 10
\end{aligned}

###### Menyelesaikan Dengan Eliminasi Gauss :
1. Tulis terlebih dahulu dalam bentuk Matriks Augmented

\begin{bmatrix} 
1 & 1 & 1 & | 6 \\ 
2 & -1 & 3 & | 14 \\ 
3 & 4 & 1 & | 10 
\end{bmatrix}

* Kolom 1 --> Koefisien x
* kolom 2 --> y
* kolom 3 --> z
* kolom 4 --> Hasil

2. Membuat pivot pertama (Elemen [1,1]=1)
Dikarenakan baris pertama sudah 1,jadi tidak perlu diubah.

3. MeEliminasikan Elemen di Bawah Pivot Pertama
Nolkan elemen dibawah x pada kolom pertama yaitu (baris 2 dan 3)

* baris 2:
$R_2 = R_2 - 2R_1$
* baris 3:
$R_3 = R_3 - 3R_1$

Matriks setelah dieliminasi:

\begin{bmatrix} 
1 & 1 & 1 & | 6 \\ 
0 & -3 & 1 & | 2 \\ 
0 & 1 & -2 & | -8 
\end{bmatrix}

4. Membuat Pivot Kedua (Elemen[2,2]=1)
elemen [2,2] dijadikan 1 dengan membagi baris dengan -3:

$R_2 = \frac{R_2}{-3}$

Hasil:

\begin{bmatrix}
1 & 1 & 1 & | 6 \\
0 & 1 & -\frac{1}{3} & |-\frac{2}{3} \\
0 & 1 & -2 & |-8
\end{bmatrix} 

5. Meeliminasi Elemen di Bawah Pivot Kedua
Nolkan Elemen di bawah pivot kedua dengan operasi:
$R_3 = R_3 - R_2$

Matriks setelah dieliminasi:

\begin{bmatrix}
1 & 1 & 1 & | 6 \\
0 & 1 & -\frac{1}{3} & |-\frac{2}{3} \\
0 & 1 & -\frac{5}{3}& |-\frac{22}{3}
\end{bmatrix} 

6. Menyelesaikan Dengan Substitusi Balik
* baris 3:
$\frac{-5}{3} z = \frac{-22}{3}$
$z=\frac{22}{5} = 4.4$
* baris 2:
$y-\frac{1}{3}(4.4) z = -\frac{2}{3}$
$y-1.47 = -0.67$
$y=0.8$
* baris 1:
$x+y+z=6$
$x+0.8+4.4=6$
$x=6-5.2=0.8$

Solusi Akhir:
$\boxed{(x, y, z) = (0.8, 0.8, 4.4)}$










