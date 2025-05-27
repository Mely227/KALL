---
title: Sistem Persamaan Linier

---

## Sistem Persamaan Linier
Sistem Persamaan Linier adalah kumpulan dua atau lebih persamaan linier yang memiliki variabel yang sama, dan solusi dari sistem tersebut adalah nilai variabel yang memenuhi semua persamaan secara bersamaan.

* Contoh SPL 

$$\begin{aligned}
    x + 2y + z &= 9 \\
    2x + y - z &= 3 \\
    3x - y + 2z &= 8
\end{aligned}$$


* Metode Penyelesaian
Substitusi, eliminasi, matriks, atau eliminasi Gauss.

1. Eliminasi Gauss
Eliminasi Gauss adalah metode untuk menyelesaikan sistem persamaan linear dengan mengubahnya ke bentuk eselon baris menggunakan operasi baris elementer.
Metode ini mempermudah penyelesaian SPL dengan menghilangkan variabel secara bertahap hingga tersisa satu variabel yang bisa disubstitusi kembali.

* Langkah-Langkah Eliminasi Gauss
1. Tulis Matriks Augmentasi
-Ubah SPL menjadi matriks augmentasi.
-Contoh:

$$\begin{aligned}
    x + 2y + z &= 9 \\
    2x + y - z &= 3 \\
    3x - y + 2z &= 8
\end{aligned}$$

*Menjadi*

$$\begin{bmatrix} 
1 & 2 & 1 & | 9 \\ 
2 & 1 & -1 & | 3 \\ 
3 & -1 & 2 & | 8 
\end{bmatrix}$$

2. Bentuk eslon Baris
-Gunakan Operasi Baris Elementer (OBE) untuk menghasilkan bentuk eselon baris:
* Elemen pivot (elemen pertama non-nol pada suatu baris) harus berada di kanan elemen pivot baris sebelumnya.
* Baris nol (jika ada) berada di bawah baris non-nol.

3. Subtitusi Balik
-Setelah matriks dalam bentuk eselon baris, lakukan substitusi balik untuk menemukan nilai variabel


##### SPL 3 PERSAMAAN
* Sistem dengan Satu Solusi : 

$$\begin{aligned}
    x + y + z &= 6 \\
    2x +3y + z &= 14 \\
    3x + 2y + 2z &= 17
\end{aligned}$$

* Penyelesaian:
1.  dalam bentuk Matriks Augmented

$$\begin{bmatrix} 
1 & 1 & 1 & | 6 \\ 
2 & 3 & 1 & | 13 \\ 
3 & 2 & 2 & | 17 
\end{bmatrix}$$

2. Eliminasi Gauss:
* Kurangi baris 2 dengan 2 x baris 1:

$$\begin{bmatrix} 
1 & 1 & 1 & | 6 \\ 
0 & 1 & -1 & | 1 \\ 
3 & 2 & 2 & | 17 
\end{bmatrix}$$

* Kurangi baris 3 dengan 3 x baris 1:

$$\begin{bmatrix} 
1 & 1 & 1 & | 6 \\ 
0 & 1 & -1 & | 1 \\ 
0 & -1 & -1 & | -1 
\end{bmatrix}$$

* Tambahkan baris 3 dengan baris 2:

$$\begin{bmatrix} 
1 & 1 & 1 & | 6 \\ 
0 & 1 & -1 & | 1 \\ 
0 & 0 & -2 & | 0
\end{bmatrix}$$

3. Substitusi Balik:
* Dari baris 3:
$2z = 0 \Rightarrow z = 0.$
* Dari baris 2:
$y-z=1 \Rightarrow y-0=1 \Rightarrow y=1$
* Dari baris 1:
$x+y+z=6 \Rightarrow x+1+0=6 \Rightarrow x=5$

4. Solusi: 
$(x,y,z)=(5,1,0)$

Sistem Memiliki **satu solusi unik**

5. Gambar Geogebra

<iframe scrolling="no" title="Satu Solusi (Berpotongan)" src="https://www.geogebra.org/material/iframe/id/mrkw38a5/width/1272/height/546/border/888888/sfsb/true/smb/false/stb/false/stbh/false/ai/false/asb/false/sri/false/rc/false/ld/false/sdz/false/ctl/false" width="1272px" height="546px" style="border:0px;"> </iframe>


* Sistem dengan Solusi Tak Hingga: 

$$\begin{aligned}
    x + 2y + z &= 5 \\
    2x +4y + z &= 10 \\
    3x + 6y + 3z &= 13
\end{aligned}$$

* Penyelesaian:
1.  dalam bentuk Matriks Augmented

$$\begin{bmatrix} 
1 & 2 & 1 & | 5 \\ 
2 & 4 & 2 & | 10 \\ 
3 & 6 & 3 & | 15 
\end{bmatrix}$$

2. Eliminasi Gauss:
* Kurangi baris 2 dengan 2 x baris 1:

$$\begin{bmatrix} 
1 & 2 & 1 & | 5 \\ 
0 & 0 & 0 & | 0 \\ 
3 & 6 & 3 & | 15 
\end{bmatrix}$$

* Kurangi baris 3 dengan 3 x baris 1:

$$\begin{bmatrix} 
1 & 2 & 1 & | 5\\ 
0 & 0 & 0 & | 0 \\ 
0 & 0 & 0 & | 0
\end{bmatrix}$$

3. Analisis:

* Baris 2 dan baris 3 semuanya nol, menunjukkan bahwa sistem memiliki **solusi tak hingga**.

* Variabel bebas: 
$y dan z$

4. Solusi Umum:
Dari baris 1: $x+2y+z=5$,kita dapat menyatakan $x$ dalam bentuk $ydanz$:
$x=5-2y-z$

Solusi umum:
$(x,y,z)=(5-2a-b,a,b)$

5. Gambar Geogebra
<iframe scrolling="no" title="Solusi Tak Hingga" src="https://www.geogebra.org/material/iframe/id/ayyuvd9d/width/1272/height/546/border/888888/sfsb/true/smb/false/stb/false/stbh/false/ai/false/asb/false/sri/false/rc/false/ld/false/sdz/false/ctl/false" width="1272px" height="546px" style="border:0px;"> </iframe>

* Sistem Tanpa Solusi : 

$$\begin{aligned}
    x + y + z &= 6 \\
    2x +3y + z &= 13 \\
    3x + 4y + 2z &= 20
\end{aligned}$$

* Penyelesaian:
1.  dalam bentuk Matriks Augmented

$$\begin{bmatrix} 
1 & 1 & 1 & | 6 \\ 
2 & 3 & 1 & | 13 \\ 
3 & 4 & 2 & | 20
\end{bmatrix}$$

2. Eliminasi Gauss:
* Kurangi baris 2 dengan 2 x baris 1:

$$\begin{bmatrix} 
1 & 1 & 1 & | 6 \\ 
0 & 1 & -1 & | 1 \\ 
3 & 4 & 2 & | 20 
\end{bmatrix}$$

* Kurangi baris 3 dengan 3 x baris 1:

$$\begin{bmatrix} 
1 & 1 & 1 & | 6 \\ 
0 & 1 & -1 & | 1 \\ 
0 & 1 & -1 & | 2 
\end{bmatrix}$$

* Tambahkan baris 3 dengan baris 2:

$$\begin{bmatrix} 
1 & 1 & 1 & | 6 \\ 
0 & 1 & -1 & | 1 \\ 
0 & 0 & 0 & | 1
\end{bmatrix}$$

3. Analisis:
* Baris 3 menunjukkan $0=1$, yang tidak mungkin. Ini berarti sistem **tidak memiliki solusi**.

4. Gambar Geogebra
<iframe scrolling="no" title="Tanpa Solusi" src="https://www.geogebra.org/material/iframe/id/ewttf4f4/width/630/height/538/border/888888/sfsb/true/smb/false/stb/false/stbh/false/ai/false/asb/false/sri/false/rc/false/ld/false/sdz/false/ctl/false" width="630px" height="538px" style="border:0px;"> </iframe>


## Matriks Invers
Matriks Invers adalah matriks yang jika dikalikan dengan matrikd aslinya menghasilkan matriks identitas.jika $A$ adalah matriks persegi berukuran $n x n$,maka invers dari $A$, yang dinotasikan sebagai $A^1$,memenuhi persamaan berikut:
$A x A^1=A^1 x A = I$

* Tugas Matriks Invers (1,0,0)
1. Langkah 1 membuat 3 persamaan variabel

$$
\begin{cases}  
4x_1 + 3x_2 - 2x_3 = 4 \\  
-5x_1 + 6x_2 + x_3 = -5 \\  
3x_1 - 2x_2 - 4x_3 = 3  
\end{cases}
$$

2. Langkah 2 ubah persamaan menjadi matriks

$$
A =
\begin{bmatrix}  
4 & 3 & -2 \\  
-5 & 6 & 1 \\  
3 & -2 & -4  
\end{bmatrix}
$$

$$
X =
\begin{bmatrix}  
x_1 \\  
x_2 \\  
X_3  
\end{bmatrix}
$$

$$
B =
\begin{bmatrix}  
4 \\  
-5 \\  
3  
\end{bmatrix}
$$

3. Langkah 3 Mencari invers $A^-1$
dengan Rumus:

$$
A^{-1} \times B =
\begin{bmatrix}
1 \\
0 \\
0
\end{bmatrix}
$$

4. Langkah 4 Menghitung Matriks Invers $A^1$

Selanjutnya untuk mencari $X$,kita menggunakan metode matriks invers,yaitu:

$$
X = A^{-1}B 
$$

Mencari invers dari matriks A yaitu dengan metode adjoin dan determinan atau redukasi baris.Hasil dari matriks A yaitu:

$$
A^{-1} =
\begin{bmatrix}  
\frac{6}{19} & \frac{-3}{19} & \frac{2}{19} \\  
\frac{5}{19} & \frac{4}{19} & \frac{1}{19} \\  
\frac{3}{19} & \frac{-2}{19} & \frac{-9}{19}  
\end{bmatrix}
$$

5. Langkah 5 Menghitung $X = A^{-1}B$
selanjutnya hitung satu persatu dengan yang $B$

$$
X =
\begin{bmatrix}  
\frac{6}{19} & \frac{-3}{19} & \frac{2}{19} \\  
\frac{5}{19} & \frac{4}{19} & \frac{1}{19} \\  
\frac{3}{19} & \frac{-2}{19} & \frac{-9}{19}  
\end{bmatrix}
\begin{bmatrix}  
4 \\  
-5 \\  
3  
\end{bmatrix}
$$

Hitung satu per satu:

$$
x_1 = \left( \frac{6}{19} \times 4 \right) + \left( \frac{-3}{19} \times (-5) \right) + \left( \frac{2}{19} \times 3 \right)
$$

$$
= \frac{24}{19} + \frac{15}{19} + \frac{6}{19} = \frac{45}{19} = 1
$$

$$
x_2 = \left( \frac{5}{19} \times 4 \right) + \left( \frac{4}{19} \times (-5) \right) + \left( \frac{1}{19} \times 3 \right)
$$

$$
= \frac{20}{19} - \frac{20}{19} + \frac{3}{19} = 0
$$

$$
x_3 = \left( \frac{3}{19} \times 4 \right) + \left( \frac{-2}{19} \times (-5) \right) + \left( \frac{-9}{19} \times 3 \right)
$$

$$
= \frac{12}{19} + \frac{10}{19} - \frac{27}{19} = 0
$$

###### 6 Maka solusi akhirnya 
hasilnya adalah:

$$
X =
\begin{bmatrix}  
1 \\  
0 \\  
0  
\end{bmatrix}
$$

sehingga hasilnya:

$$
x_1 = 1, \quad x_2 = 0, \quad x_3 = 0
$$


## Ringkasan dan Tugas [Transformasi Matriks]

Transformasi Matriks adalah Bayangin kamu punya vektor (misalnya panah yang nunjuk ke suatu arah) terus kamu "ubah" bentuk atau arahnya pakai aturan tertentu. Nah, kalau aturan itu bisa ditulis pakai perkalian matriks, itu disebut.Dengan menggunakan matriks $A$ berukuran $m$ X $n$ bisa digunakan untuk mendefinisikan sebuah fungsi $T$ yang mengambil vektor kolom $\vec{x}$ adalah vektor kolom berukuran $n \times 1$ dan menghasilkan vektor kolom $\vec{y}$ berukuran $m \times 1$ melalui persamaan:
$$
\vec{y} = T(\vec{x}) = A\vec{x}
$$

Fungsi ini disebut *Transformasi Matriks, dan termasuk dalam kelas umum yang biasanya disebut **Transformasi Linier* yaitu fungsi antar vektor

---

* Perkalian Matriks - Vektor

Agar hasil perkalian tetap berupa vektor  2D $(\ \mathbb{R}^2)$, maka matriks $A$ harus berukuran $2$ X $2$. 
Diberikan matriks $A$ dan tiga vektor $\vec{x},\ \vec{y},\ \vec{z}$ hasil perkalian antara matriks dan vektor dihitung sebagai berikut:
$$
A = \begin{bmatrix}
4 & 2 \\
1 & 3
\end{bmatrix}, \quad
\vec{x} = \begin{bmatrix}
1 \\
1
\end{bmatrix}, \quad
\vec{y} = \begin{bmatrix}
-1 \\
1
\end{bmatrix}, \quad
\vec{z} = \begin{bmatrix}
3 \\
-1
\end{bmatrix}
$$


Solusi:
$$
A\vec{x} = \begin{bmatrix}
5 \\
5
\end{bmatrix}, \quad
A\vec{y} = \begin{bmatrix}
-3 \\
1
\end{bmatrix}, \quad
A\vec{z} = \begin{bmatrix}
-1 \\
3
\end{bmatrix}
$$


Perkalian matriks mengubah panjang dan arah vektor dalam contoh di atas vektor $\vec{x}$ dan $A\vec{x}$ memiliki arah yang sama tapi panjangnya yang berubah. Namun, $\vec{y}$ dan $\vec{z}$ beruubah arah saat dikalikan dengan $A$. Hal ini menunjukkan bahwa matriks bertindak secara berbeda terhadap vektor yang berbeda.

---

* Menggabungkan penjumlahan dan perkalian matriks

Diketahui:

$$
A = \begin{bmatrix}
1 & 1 \\
1 & 2
\end{bmatrix}, \quad
\vec{x} = \begin{bmatrix}
2 \\
1
\end{bmatrix}, \quad
\vec{y} = \begin{bmatrix}
-1 \\
1
\end{bmatrix}
$$


Sketsa: $\vec{x} + \vec{y}$,$A\vec{x}$,$A\vec{y}$ dan $A(\vec{x}+\vec{y})$
langkah ini bertujuan untuk melihat bagaimana penjumlahan vektor berinteraksi dengan transformasi matriks.

Dihitung:

$$
\vec{x} + \vec{y} = \begin{bmatrix}
1 \\
2
\end{bmatrix}, \quad
A\vec{x} = \begin{bmatrix}
3 \\
4
\end{bmatrix}, \quad
A\vec{y} = \begin{bmatrix}
0 \\
1
\end{bmatrix}, \quad
A(\vec{x} + \vec{y}) = \begin{bmatrix}
3 \\
5
\end{bmatrix}
$$


Ini menunjukkan *sifat distributif* dari perkalian matriks terhadap penjumlahan vektor: $$A(\vec{x} + \vec{y}) = A\vec{x} + A\vec{y}$$

---

* Menggambar Efek dari Perkalian matriks

Diketahui:

$$
A = \begin{bmatrix}
1 & 1 \\
-1 & -1
\end{bmatrix}, \quad
\vec{x} = \begin{bmatrix}
1 \\
1
\end{bmatrix}, \quad
\vec{y} = \begin{bmatrix}
-1 \\
1
\end{bmatrix}, \quad
\vec{z} = \begin{bmatrix}
4 \\
4
\end{bmatrix}
$$


Solusi:

$$
A\vec{x} = \begin{bmatrix}
0 \\
0
\end{bmatrix} \quad 
A\vec{y} = \begin{bmatrix}
-2 \\
-2
\end{bmatrix} \quad
and \quad
A\vec{z} = \begin{bmatrix}
3 \\
3\end{bmatrix}
$$

Beberapa vektor seperti $(\vec{x}$ dan $\vec{y})$ setelah dikalikan dengan matriks, hasilnya adalah vektor nol sementara vektor lain tetepa berada pada garis tertentu.

---

* Transformasi terhadap bidang kartesius

Pada bagian ini memeperkenalkan transisi dan menggambarkan vektor satu per satu ke menggambarkan bagaimana seluruh bidang katresius $(\ \mathbb{R}^2)$berubah oleh matriks.

* Visualisasi Transformasi Matriks Menggunnakan vektor

efek transformasi terhadap seluruh bidang Kartesius dengan melihat bagaimana *persegi satuan (unit square)* berubah.
Misalkan: 

$$
A = \begin{bmatrix}
1 & 4 \\
2 & 3
\end{bmatrix}
$$


Titik - titik sudut dari persegi satuan berada di:

$$
\begin{bmatrix}
0 \\
0
\end{bmatrix}, \quad
\begin{bmatrix}
1 \\
0
\end{bmatrix}, \quad
\begin{bmatrix}
1 \\
1
\end{bmatrix}, \quad
\begin{bmatrix}
0 \\
1
\end{bmatrix}
$$


Setelah dikalikan deng $A$, titik - titik tersebut menjadi:


$$
\begin{bmatrix}
0 \\
0
\end{bmatrix}, \quad
\begin{bmatrix}
1 \\
2
\end{bmatrix}, \quad
\begin{bmatrix}
5 \\
5
\end{bmatrix}, \quad
\begin{bmatrix}
4 \\
3
\end{bmatrix}
$$

 Adapun tips cepat untuk menggunakan matriks kolom: 
 Buat matriks $B$ yang kolom - kolomnya adalah titik - titik sudut:


$$
B = \begin{bmatrix}
0 & 1 & 1 & 0 \\
0 & 0 & 1 & 1
\end{bmatrix}
$$


Dikalikan:

$$
AB = \begin{bmatrix}
0 & 2 & 6 & 4 \\
0 & 1 & 4 & 3
\end{bmatrix}
$$


Proses ini cepat jika harus dilakukan transformasi pada banyak titik sekaligus

Perubahan bentuk dari persegi satuan setelah dikalikan dengan matriks:

$$
A = \begin{bmatrix}
1 & 4 \\
2 & 3
\end{bmatrix}
$$ 


## Transformasi Linier

##### Pengertian
Transformasi linier adalah pemetaan (fungsi) dari satu ruang vektor ke ruang vektor lain yang mempertahankan operasi penjumlahan dan perkalian skalar.
Bentuk umum :
$T: \mathbb{R}^n \to \mathbb{R}^m$

##### Syarat Transformasi Linier
Sebuah fungsi $T (v)$adalah transformasi linier jika untuk semua vektor $u,v$ dan skalar *c*,berlaku:

1. Penjumlahan vektor:
$T(u+v)=T(u)+T(v)$

2. Perkalian skalar:
$T(c v)=cT(v)$
Kalau kedua syarat di atas terpenuhi, maka 𝑇 adalah transformasi linier.

##### Tugas 1  Membuktikan bahwa $T(v1,v2)=(v1+v2,v1)$ adalah transformasi Linier

##### Jawaban
Transformasi $T(v1,v2)=(v1+v2,v1)$ didefinisikan sebagai:
$T(v1,v2)=(v1+v2,v1)$

Misalkan:

${u} = (u_1, u_2), \quad \mathbf{v} = (v_1, v_2)$

1. Cek Penjumlahan :

\begin{align*}
T(\mathbf{u} + \mathbf{v}) &= T((u_1 + v_1, u_2 + v_2)) \\
&= ((u_1 + v_1) + (u_2 + v_2), u_1 + v_1) \\
&= (u_1 + v_1 + u_2 + v_2, u_1 + v_1)
\end{align*}

Sementara itu:

$T(\mathbf{u}) = (u_1 + u_2, u_1), \quad T(\mathbf{v}) = (v_1 + v_2, v_1)$

$T(\mathbf{u}) + T(\mathbf{v}) = (u_1 + u_2 + v_1 + v_2, u_1 + v_1)$

Karena:

$ T(\mathbf{u} + \mathbf{v}) = T(\mathbf{u}) + T(\mathbf{v})$

2. Cek Perkalian Skalar:

\begin{align*}
T(c\mathbf{v}) &= T(cv_1, cv_2) \\
&= (cv_1 + cv_2, cv_1) \\
&= c(v_1 + v_2, v_1) \\
&= cT(\mathbf{v})
\end{align*}

3. Kesimpulan
Karena kedua sifat di atas dipenuhi, maka:

$T(v_1, v_2) = (v_1 + v_2, v_1) \text{ adalah transformasi linier.}$


##### Tugas 2  cari matriks rotasi,refleksi,shear,scala


1. Reflection about the x-axis
Matriks transformasi:


$\begin{bmatrix}
1 & 0 \\
0 & -1
\end{bmatrix}$


Contoh titik:

$
(2, 3) \rightarrow (2, -3) 
$

Gambar GeoGebra:

<iframe scrolling="no" title="Gambar 1" src="https://www.geogebra.org/material/iframe/id/xhfraxhe/width/1272/height/594/border/888888/sfsb/true/smb/false/stb/false/stbh/false/ai/false/asb/false/sri/false/rc/false/ld/false/sdz/false/ctl/false" width="1272px" height="594px" style="border:0px;"> </iframe>



2. Reflection about the y-axis
Matriks transformasi:


$\begin{bmatrix}
-1 & 0 \\
0 & 1
\end{bmatrix}$


Contoh titik:

$
(3, 2) \rightarrow (-3, 2) 
$

Gambar GeoGebra:

<iframe scrolling="no" title="Gambar 2" src="https://www.geogebra.org/material/iframe/id/jxtushsj/width/630/height/586/border/888888/sfsb/true/smb/false/stb/false/stbh/false/ai/false/asb/false/sri/false/rc/false/ld/false/sdz/false/ctl/false" width="630px" height="586px" style="border:0px;"> </iframe>


3. Reflection about the line $y = x$
Matriks transformasi:



$\begin{bmatrix}
0 & 1 \\
1 & 0
\end{bmatrix}$



Contoh titik:

$
(5, 7) \rightarrow (7, 5) 
$

Gambar GeoGebra:

<iframe scrolling="no" title="Gambar 3" src="https://www.geogebra.org/material/iframe/id/xwmzkx6q/width/630/height/586/border/888888/sfsb/true/smb/false/stb/false/stbh/false/ai/false/asb/false/sri/false/rc/false/ld/false/sdz/false/ctl/false" width="630px" height="586px" style="border:0px;"> </iframe>


4. Reflection about the line $y = -x$
Matriks transformasi:


$\begin{bmatrix}
0 & -1 \\
-1 & 0
\end{bmatrix}$


Contoh titik:

$
(3, 1) \rightarrow (-1, -3) 
$

Gambar GeoGebra:

<iframe scrolling="no" title="Gambar 4" src="https://www.geogebra.org/material/iframe/id/r9ujtmxc/width/630/height/586/border/888888/sfsb/true/smb/false/stb/false/stbh/false/ai/false/asb/false/sri/false/rc/false/ld/false/sdz/false/ctl/false" width="630px" height="586px" style="border:0px;"> </iframe>



5. Reflection about the origin
Matriks transformasi:


$\begin{bmatrix}
-1 & 0 \\
0 & -1
\end{bmatrix}$


Contoh titik:

$
(6, -3) \rightarrow (-6, 3) 
$

Gambar Geogebra:

<iframe scrolling="no" title="Gambar 5" src="https://www.geogebra.org/material/iframe/id/rpcufcnz/width/630/height/586/border/888888/sfsb/true/smb/false/stb/false/stbh/false/ai/false/asb/false/sri/false/rc/false/ld/false/sdz/false/ctl/false" width="630px" height="586px" style="border:0px;"> </iframe>


##### Refleksi Sumbu X=2

```python=
import numpy as np
import matplotlib.pyplot as plt
from mpl_toolkits.mplot3d import Axes3D

# Titik-titik objek asli (misalnya, segitiga 3D)
points = np.array([
    [2, 3, 1],
    [1, 4, 3],
    [4, 2, 1]
]).T  # bentuknya 3xN

# Matriks refleksi terhadap bidang x = 0
reflection_matrix = np.array([
    [-1, 0, 0],
    [ 0, 1, 0],
    [ 0, 0, 1]
])

# Langkah-langkah untuk refleksi terhadap bidang x = 2:
# 1. Translasi ke kiri sejauh 2 satuan (x -= 2)
translated_points = points.copy()
translated_points[0] -= 2

# 2. Refleksi terhadap bidang x = 0
reflected_translated = reflection_matrix @ translated_points

# 3. Translasi kembali ke kanan sejauh 2 satuan (x += 2)
reflected_points = reflected_translated.copy()
reflected_points[0] += 2

# Buat plot
fig = plt.figure()
ax = fig.add_subplot(111, projection='3d')

# Gambar objek asli (biru)
ax.plot(points[0], points[1], points[2], 'bo-', label='Asli')

# Gambar objek setelah refleksi (merah)
ax.plot(reflected_points[0], reflected_points[1], reflected_points[2], 'ro-', label='Refleksi')

# Tambahkan bidang bantu di x = 2
x_plane = np.full((2, 2), 2)  # bidang x = 2
y_plane, z_plane = np.meshgrid(np.linspace(0, 3, 2), np.linspace(0, 3, 2))
ax.plot_surface(x_plane, y_plane, z_plane, alpha=0.2, color='gray')

# Set aspek dan label
ax.set_xlabel('X')
ax.set_ylabel('Y')
ax.set_zlabel('Z')
ax.set_title('Refleksi terhadap bidang x = 2')
ax.legend()
ax.set_box_aspect([1,1,1])  # aspek rasio 1:1:1

plt.show()
```
![image](https://hackmd.io/_uploads/SyeTegffel.png)


##### Refleksi Sumbu y=2

```python=
import numpy as np
import matplotlib.pyplot as plt
from mpl_toolkits.mplot3d import Axes3D

# Titik-titik objek asli (misalnya, segitiga 3D)
points = np.array([
    [1, 1, 1],
    [2, 1, 1],
    [1.5, 2, 1]
]).T  # bentuknya 3xN

# Matriks refleksi terhadap bidang y = 0
reflection_matrix = np.array([
    [1,  0, 0],
    [0, -1, 0],
    [0,  0, 1]
])

# Langkah-langkah untuk refleksi terhadap bidang y = 2:
# 1. Translasi ke bawah sejauh 2 satuan (y -= 2)
translated_points = points.copy()
translated_points[1] -= 2

# 2. Refleksi terhadap bidang y = 0
reflected_translated = reflection_matrix @ translated_points

# 3. Translasi kembali ke atas sejauh 2 satuan (y += 2)
reflected_points = reflected_translated.copy()
reflected_points[1] += 2

# Buat plot
fig = plt.figure()
ax = fig.add_subplot(111, projection='3d')

# Gambar objek asli (biru)
ax.plot(points[0], points[1], points[2], 'bo-', label='Asli')

# Gambar objek setelah refleksi (merah)
ax.plot(reflected_points[0], reflected_points[1], reflected_points[2], 'ro-', label='Refleksi')

# Tambahkan bidang bantu di y = 2
y_plane = np.full((2, 2), 2)  # bidang y = 2
x_plane, z_plane = np.meshgrid(np.linspace(0, 3, 2), np.linspace(0, 3, 2))
ax.plot_surface(x_plane, y_plane, z_plane, alpha=0.2, color='gray')

# Set aspek dan label
ax.set_xlabel('X')
ax.set_ylabel('Y')
ax.set_zlabel('Z')
ax.set_title('Refleksi terhadap bidang y = 2')
ax.legend()
ax.set_box_aspect([1,1,1])  # aspek rasio 1:1:1

plt.show()
```

![image](https://hackmd.io/_uploads/Hkl-blffee.png)


##### Refleksi Sumbu y=x

```python=
import numpy as np
import matplotlib.pyplot as plt
from mpl_toolkits.mplot3d import Axes3D

# Titik-titik objek asli (misalnya, segitiga 3D)
points = np.array([
    [1, 4, 2],
    [2, 3, 4],
    [3, 2, 1]
]).T  # bentuknya 3xN

# Matriks refleksi terhadap bidang y = x
reflection_matrix = np.array([
    [0, 1, 0],
    [1, 0, 0],
    [0, 0, 1]
])

# Lakukan refleksi
reflected_points = reflection_matrix @ points

# Buat plot
fig = plt.figure()
ax = fig.add_subplot(111, projection='3d')

# Gambar objek asli (biru)
ax.plot(points[0], points[1], points[2], 'bo-', label='Asli')

# Gambar objek setelah refleksi (merah)
ax.plot(reflected_points[0], reflected_points[1], reflected_points[2], 'ro-', label='Refleksi')

# Tambahkan bidang bantu y = x di bidang z = 0–3
x_vals, y_vals = np.meshgrid(np.linspace(0, 3, 2), np.linspace(0, 3, 2))
z_vals = np.zeros_like(x_vals)
ax.plot_surface(x_vals, y_vals, z_vals, alpha=0.1, color='gray')

# Tambahkan garis bantu bidang y = x (di z = 0)
ax.plot([0, 3], [0, 3], [0, 0], 'k--', label='Bidang y = x (z=0)')

# Set aspek dan label
ax.set_xlabel('X')
ax.set_ylabel('Y')
ax.set_zlabel('Z')
ax.set_title('Refleksi terhadap bidang y = x')
ax.legend()
ax.set_box_aspect([1,1,1])  # aspek rasio 1:1:1

plt.show()
```

![image](https://hackmd.io/_uploads/rJkrWefMlx.png)


## Definisi Eigenvalue Eigenvector 

Eigenvalue atau Nilai eigen adalah Skalar yang digunakan untuk mengubah atau meregangkan vektor Eigen. Vektor eigen dan nilai eigen berkisar pada konsep matriks.Matriks digunakan dalam masalah pembelajaran mesin untuk mewakili sekumpulan besar informasi. Nilai eigen dan vektor eigen adalah tentang membangun satu vektor dengan satu nilai untuk mewakili matriks besar
* Misalkan  $A$ adalah matriks persegi misal $(n x n)$ ,maka Vektor tak nol $v$ disebut eigenvector dari $A$ ,jika :

$$ A \mathbf{v} = \lambda \mathbf{v} $$

Dimana:
* $A$ = Matriks
* $v$ = eigenvektor
* $\lambda$ = eigenvalue (skalar)

 Artinya,tranformasi matriks $A$ terhadap vekbor $v$ hanya mengubah skala vektor tersebut dikali dengan $\lambda$ ,arahnya tetap

##### Mencari **eigenvalue** dan **eigenvector** dari matriks:

$A = \begin{bmatrix} 2 & -1 \\ 4 & 3 \end{bmatrix}$

---

**Langkah 1: Mencari Eigenvalue**

Gunakan persamaan karakteristik:

$\det(A - \lambda I) = 0$

Kurangkan $\lambda I$ dari $A$:

$A - \lambda I = \begin{bmatrix} 2 - \lambda & -1 \\ 4 & 3 - \lambda \end{bmatrix}$

Hitung determinan:

$\begin{aligned}
\det(A - \lambda I) &= (2 - \lambda)(3 - \lambda) - (-1)(4) \\
&= (2 - \lambda)(3 - \lambda) + 4 \\
&= \lambda^2 - 5\lambda + 10
\end{aligned}$

Selesaikan persamaan kuadrat:

$\lambda = \frac{5 \pm \sqrt{(-5)^2 - 4(1)(10)}}{2(1)} = \frac{5 \pm \sqrt{-15}}{2} = \frac{5}{2} \pm \frac{i\sqrt{15}}{2}$

Jadi, dua nilai eigen:

$\lambda_1 = \frac{5}{2} + \frac{i\sqrt{15}}{2}$  
$\lambda_2 = \frac{5}{2} - \frac{i\sqrt{15}}{2}$

---

**Langkah 2: Mencari Eigenvector**

Gunakan nilai $\lambda_2 = \frac{5}{2} - \frac{i\sqrt{15}}{2}$

Matriks $A - \lambda_2 I$:

$\begin{bmatrix}
\frac{-1}{2} + \frac{i\sqrt{15}}{2} & -1 \\
4 & \frac{3}{2} + \frac{i\sqrt{15}}{2}
\end{bmatrix}$

Misal vektor eigen berbentuk:

$\vec{v} = \begin{bmatrix} x \\ 1 \end{bmatrix}$

Gunakan baris pertama:

$\left( \frac{-1}{2} + \frac{i\sqrt{15}}{2} \right)x - 1 = 0$

Selesaikan:

$x = \frac{1}{\frac{-1}{2} + \frac{i\sqrt{15}}{2}} = \frac{2}{-1 + i\sqrt{15}}$

Rasionalisasi:

$x = \frac{2(-1 - i\sqrt{15})}{(-1 + i\sqrt{15})(-1 - i\sqrt{15})} = \frac{-2 - 2i\sqrt{15}}{16} = \frac{-1 - i\sqrt{15}}{8}$

Maka, vektor eigen untuk $\lambda_2$:

$\vec{v}_2 = \begin{bmatrix} \frac{-1 - i\sqrt{15}}{8} \\ 1 \end{bmatrix}$

---

**Kesimpulan:**

- Eigenvalue:  
  $\lambda_1 = \frac{5}{2} + \frac{i\sqrt{15}}{2}$  
  $\lambda_2 = \frac{5}{2} - \frac{i\sqrt{15}}{2}$

- Eigenvector untuk $\lambda_2$:  
  $\vec{v}_2 = \begin{bmatrix} \frac{-1 - i\sqrt{15}}{8} \\ 1 \end{bmatrix}$

```python=
# Code untuk Konfirmasi
import numpy as np
from numpy import linalg as LA
input = np.array([[2,-1],[4,3]])
w, v = LA.eig(input)
print(w)
print(v)
```
```python=
Output:
[2.5+1.93649167j 2.5-1.93649167j]
[[ 0.1118034 -0.4330127j  0.1118034 +0.4330127j]
 [-0.89442719+0.j        -0.89442719-0.j       ]]
```


##### Ortogonal & Ortonormal

1. **Ortogonal**  
Dua vektor dikatakan ortogonal jika hasil *dot product* (perkalian titik) antara keduanya adalah nol.  
Secara matematis, jika ada dua vektor $u$ dan $v$, maka:

$u \cdot v = 0$

Artinya:
- Vektor $u$ dan $v$ saling tegak lurus (membentuk sudut 90°).
- Tidak harus memiliki panjang (norma) tertentu.

2. **Ortonormal**  
Sekumpulan vektor dikatakan ortonormal jika mereka ortogonal satu sama lain **dan** masing-masing memiliki panjang (norma) 1.

Syarat ortonormal:
- Ortogonal antar vektor: $u \cdot v = 0$ jika $u \ne v$
- Norma 1 untuk setiap vektor: $||u|| = 1$

Misal $\vec{u}, \vec{v} \in \mathbb{R}^n$, maka:

$\vec{u} \cdot \vec{v} = 0$ jika $\vec{u} \ne \vec{v}$  
$||\vec{u}|| = 1$ dan $||\vec{v}|| = 1$

---

**Contoh:**  
Misalkan kita punya matriks simetris 2x2:

$A = \begin{bmatrix} 4 & 1 \\ 1 & 3 \end{bmatrix}$

**Langkah: Cari Eigenvalue**  
Hitung determinan:

$\det(A - \lambda I) = \left| \begin{array}{cc} 4 - \lambda & 1 \\ 1 & 3 - \lambda \end{array} \right| = (4 - \lambda)(3 - \lambda) - 1 = 0$

Maka:

$\lambda^2 - 7\lambda + 11 = 0$

Gunakan rumus kuadrat:

$\lambda = \frac{7 \pm \sqrt{49 - 44}}{2} = \frac{7 \pm \sqrt{5}}{2}$

Jadi:

$\lambda_1 = \frac{7 + \sqrt{5}}{2}, \quad \lambda_2 = \frac{7 - \sqrt{5}}{2}$

---

**Langkah: Cari Eigenvector**  
Misal untuk $\lambda_1 \approx 5.618$:

$A - \lambda_1 I \approx \begin{bmatrix} -1.618 & 1 \\ 1 & -2.618 \end{bmatrix}$

Ambil baris pertama:

$-1.618x + y = 0 \Rightarrow y = 1.618x$

Maka vektor eigen (belum dinormalisasi):

$\vec{v}_1 = \begin{bmatrix} 1 \\ 1.618 \end{bmatrix}$

Norma:

$||\vec{v}_1|| = \sqrt{1^2 + (1.618)^2} \approx \sqrt{3.618} \approx 1.902$

Normalisasi:

$\vec{u}_1 = \frac{1}{1.902} \begin{bmatrix} 1 \\ 1.618 \end{bmatrix} \approx \begin{bmatrix} 0.526 \\ 0.851 \end{bmatrix}$

---

Lakukan hal serupa untuk $\lambda_2 \approx 1.382$:

$A - \lambda_2 I \approx \begin{bmatrix} 2.618 & 1 \\ 1 & 1.618 \end{bmatrix}$

Ambil salah satu baris:

$2.618x + y = 0 \Rightarrow y = -2.618x$

Maka vektor eigen:

$\vec{v}_2 = \begin{bmatrix} 1 \\ -2.618 \end{bmatrix}$

Norma:

$||\vec{v}_2|| = \sqrt{1^2 + (-2.618)^2} = \sqrt{7.854} \approx 2.802$

Normalisasi:

$\vec{u}_2 = \frac{1}{2.802} \begin{bmatrix} 1 \\ -2.618 \end{bmatrix} \approx \begin{bmatrix} 0.357 \\ -0.934 \end{bmatrix}$

---

**Hasil Akhir: Basis Ortonormal dari Eigenvektor**

Dua vektor ortonormal hasil normalisasi eigenvektor:

$\vec{u}_1 = \begin{bmatrix} 0.526 \\ 0.851 \end{bmatrix}, \quad \vec{u}_2 = \begin{bmatrix} 0.357 \\ -0.934 \end{bmatrix}$

Verifikasi:
1. $\vec{u}_1 \cdot \vec{u}_2 = 0$ (ortogonal)  
2. $||\vec{u}_1|| = 1$, $||\vec{u}_2|| = 1$ (norma 1)  
3. Jadi keduanya adalah **ortonormal**  
4. Dan merupakan **eigenvektor dari A**

</small>

```python=
# Kode Phython Konfirmasinya
import numpy as np

# Matriks simetris
A = np.array([[4, 1],
              [1, 3]])

# Cari eigenvalue dan eigenvektor
eigenvalues, eigenvectors = np.linalg.eig(A)

# Tampilkan hasil
print("Eigenvalue:")
print(eigenvalues)
print("\nEigenvektor (sebelum dinormalisasi):")
print(eigenvectors)

# Normalisasi eigenvektor untuk jadi ortonormal
normalized_vectors = []
for v in eigenvectors.T:  # per kolom (karena np.linalg.eig mengembalikan kolom sebagai vektor)
    norm = np.linalg.norm(v)
    normalized_vectors.append(v / norm)

# Konversi ke array NumPy
normalized_vectors = np.array(normalized_vectors)

print("\nEigenvektor yang sudah dinormalisasi (ortonormal):")
print(normalized_vectors)
```

```python=
Output:

Eigenvalue:
[4.61803399 2.38196601]

Eigenvektor (sebelum dinormalisasi):
[[ 0.85065081 -0.52573111]
 [ 0.52573111  0.85065081]]

Eigenvektor yang sudah dinormalisasi (ortonormal):
[[ 0.85065081  0.52573111]
 [-0.52573111  0.85065081]]
```

## Perkalian Titik Vektor (Dot Product)

### Pengertian
Perkalian vektor dibedakan menjadi tiga jenis yaitu perkalian vektor dengan skalar, perkalian silang (cross product), dan perkalian titik vektor (dot product).atau hasil kali titik (dot product), yang membantu kita mengukur panjang vektor dan sudut yang dibentuk oleh sepasang vektor. Untuk vektor-vektor dua dimensi v dan w, hasil kali titik (v · w) didefinisikan sebagai bilangan skalar berikut:


$$
\mathbf{v} \cdot \mathbf{w} = 
\begin{bmatrix}
v_1 \\
v_2
\end{bmatrix}
\cdot
\begin{bmatrix}
w_1 \\
w_2
\end{bmatrix}
= v_1w_1 + v_2w_2.
$$



##### Contoh Basis 2D :
Basis 2D

$$
\begin{bmatrix}
1 & 0 \\
0 & 1 \\
\end{bmatrix}
$$


Jadi


$$
\begin{bmatrix}
1 \\
0
\end{bmatrix}
\cdot
\begin{bmatrix}
0 \\
1
\end{bmatrix}
= 1.0 + 0.1 = 0
$$

Gambar Geogebra :

<iframe scrolling="no" title="Basic 2D" src="https://www.geogebra.org/material/iframe/id/khzkvtev/width/1272/height/594/border/888888/sfsb/true/smb/false/stb/false/stbh/false/ai/false/asb/false/sri/false/rc/false/ld/false/sdz/false/ctl/false" width="1272px" height="594px" style="border:0px;"> </iframe>


##### Contoh 3D : 

Basis 3D


$$
\begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{bmatrix}
$$


Jadi 

b1 = 


$$
\begin{bmatrix}
1 \\
0 \\
0
\end{bmatrix}
$$


b2 = 

$$
\begin{bmatrix}
0 \\
1 \\
0
\end{bmatrix}
$$


b3 = 

$$
\begin{bmatrix}
0 \\
0 \\
1
\end{bmatrix}
$$


Penyelesaian:


b1.b2   =  

$$
\begin{bmatrix}
1 \\
0 \\
0
\end{bmatrix}
\cdot
\begin{bmatrix}
0 \\
1 \\
0
\end{bmatrix} = (1.0) + (0.1) + (0.0) =0
$$


b1.b3   = 

$$
\begin{bmatrix}
1 \\
0 \\
0
\end{bmatrix}
\cdot
\begin{bmatrix}
0 \\
0 \\
1
\end{bmatrix} = (1.0) + (0.0) + (0.1) =0
$$


b2.b3   = 

$$
\begin{bmatrix}
0 \\
1 \\
0
\end{bmatrix}
\cdot
\begin{bmatrix}
0 \\
0 \\
1
\end{bmatrix} = (0.0) + (1.0) + (0.1) =0
$$


Gambar Geogebra :

<iframe scrolling="no" title="Basic 2D" src="https://www.geogebra.org/material/iframe/id/khzkvtev/width/1272/height/594/border/888888/sfsb/true/smb/false/stb/false/stbh/false/ai/false/asb/false/sri/false/rc/false/ld/false/sdz/false/ctl/false" width="1272px" height="594px" style="border:0px;"> </iframe>


### Geometri dari Hasil Kali Titik

Hasil kali titik (dot product) adalah operasi antara dua vektor yang menghasilkan skalar.
Rumusnya yaitu :

$$
\mathbf{v} \cdot \mathbf{w} = 
\begin{bmatrix}
v_1 \\
v_2 \\
\vdots \\
v_m
\end{bmatrix}
\cdot
\begin{bmatrix}
w_1 \\
w_2 \\
\vdots \\
w_m
\end{bmatrix}
= v_1w_1 + v_2w_2 + \ldots + v_mw_m.
$$


##### Contoh
Kita menghitung hasil kali titik antara dua vektor berdimensi empat sebagai berikut:

$$
\begin{bmatrix}
1 \\
4 \\
-2 \\
3
\end{bmatrix}
\cdot
\begin{bmatrix}
3 \\
-1 \\
0 \\
0
\end{bmatrix}
= 1(3) + 4(-1) + (-2)(0) + 5(2) = 3 - 4+0+10 = 9
$$


##### Vektor Satuan    $\mathbb{R}^n$
Misalkan 

$\mathbf{x}$ 

adalah vektor tak nol 

$\mathbb{R}^n$.

Maka :

$$\frac{\mathbf{y}}{\|\mathbf{y}\|}$$

Adalah vektor satuan

$$\frac{\mathbf{y}}{\|\mathbf{y}\|} \cdot \frac{\mathbf{y}}{\|\mathbf{y}\|} = \frac{\mathbf{y} \cdot \mathbf{y}}{\|\mathbf{y}\|^2} = \frac{\|\mathbf{y}\|^2}{\|\mathbf{y}\|^2} = 1$$


##### Contoh:
###### 1. Misalkan diberikan titik berikut:
* $A = (0,0)$
* $B = (3,0)$
* $D = (3,2)$
* $C = (3,4)$

###### 2. Vektor-vektor

* Vektor 

$$
u = AB = \begin{bmatrix}
3\\
0 \\
\end{bmatrix}
$$


* Vektor 

$$
a = AD = \begin{bmatrix}
3\\
2 \\
\end{bmatrix}
$$

* Vektor 

$$
v = AC = \begin{bmatrix}
3\\
4 \\
\end{bmatrix}
$$


###### 3. Panjang Vektor

$$
\|\vec{u}\| = \sqrt{3^2 + 0^2} = \sqrt{9} = 3
\]
\[
\|\vec{a}\| = \sqrt{3^2 + 2^2} = \sqrt{9 + 4} = \sqrt{13}
\]
\[
\|\vec{v}\| = \sqrt{3^2 + 4^2} = \sqrt{9 + 16} = \sqrt{25} = 5
$$

###### 4. Sudut antara vektor $u$ dan $a$:

Gunakan rumus dot product:

$$
\cos \theta = \frac{\vec{u} \cdot \vec{a}}{\|\vec{u}\| \|\vec{a}\|}
$$

Penyelesaian:

$$
\
\vec{u} \cdot \vec{a} = (3)(3) + (0)(2) = 9
\]
\[
\cos \theta = \frac{9}{3\sqrt{13}} = \frac{3}{\sqrt{13}} \Rightarrow \theta = \cos^{-1}\left(\frac{3}{\sqrt{13}}\right)
\]
\[
\theta \approx 33.69^\circ
\]
$$

###### 5. Vektor satuan $v$:

$$
\hat{v} = \frac{\vec{v}}{\|\vec{v}\|} = \frac{1}{5} \begin{bmatrix} 3 \\ 4 \end{bmatrix} = \begin{bmatrix} \frac{3}{5} \\ \frac{4}{5} \end{bmatrix}
$$

###### 6. Verifikasi panjang vektor satuan

$$ 
\|\hat{v}\| = \sqrt{\left( \frac{3}{5} \right)^2 + \left( \frac{4}{5} \right)^2}
= \sqrt{\frac{9}{25} + \frac{16}{25}} = \sqrt{\frac{25}{25}} = \sqrt{1} = 1
$$

###### Bukti Geogebra

<iframe scrolling="no" title="Sudut" src="https://www.geogebra.org/material/iframe/id/xpgdmx2u/width/1272/height/594/border/888888/sfsb/true/smb/false/stb/false/stbh/false/ai/false/asb/false/sri/false/rc/false/ld/false/sdz/false/ctl/false" width="1272px" height="594px" style="border:0px;"> </iframe>

