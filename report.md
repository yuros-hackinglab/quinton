# Laporan Hasil Research

<!-- Dokumen ini ditulis dalam format Markdown (.md) -->

## Background

Shelver OS merupakan sistem operasi yang dirancang secara khusus untuk mendukung kebutuhan lembaga GLAM (Gallery, Library, Archives, and Museums). Sistem ini dikembangkan dengan pendekatan fungsional dan berorientasi pada stabilitas, keberlanjutan, serta kemudahan untuk hardware dengan spesifikasi rendah dalam skala global.  

## Methods

### Pembentukan dan Pengelolaan Tim

Riset dimulai dengan pembentukan tim yang dimana awalnya ada pergantian ketua yang dilakukan secara musyawarah. Pembentukan tim dilakukan secara sukarela, tanpa ada paksaan untuk bergabung dengan tim riset shelver os. Untuk pengelolaan tim, dilakukan berdasarkan kemampuan individu, seperti kemampuan dalam melakukan instalasi kernel, desktop environment, dan browser. Testing terkait riset pun sudah dibagi kepada individu yang mampu melakukan testing.

### Proses Riset

Proses riset dilakukan secara bertahap, dimulai dari persiapan lingkungan pengujian, penentuan parameter pengukuran, hingga eksekusi pengujian. Setiap pengujian dilakukan dengan skenario yang sama untuk menjaga konsistensi data. Parameter yang diamati meliputi penggunaan sumber daya sistem, stabilitas selama penggunaan, serta respons sistem terhadap aktivitas tertentu.

Selama proses riset, seluruh aktivitas dicatat secara rinci, termasuk kondisi awal sistem, perubahan konfigurasi, dan hasil pengamatan. Dokumentasi dilakukan secara real-time untuk meminimalkan kehilangan data penting.

### kernel
#### 1. linux git

berikut hasil testing kernel pada saat tidak menjalankan aplikasi
<img src="img/linux-git-idle.png" width="800">

Di bawah ini adalah hasil testing ketika membuka aplikasi youtube dan slims
<img src="img/linux-git-using.png" width="800">


#### 2. linux lqx
berikut hasil testing kernel pada saat tidak menjalankan aplikasi
<img src="img/linux-lqx-idle.png" width="800">

Di bawah ini adalah hasil testing ketika membuka aplikasi youtube dan slims
<img src="img/linux-lqx-using.png" width="800">


#### 3 linux lts61
berikut hasil testing kernel pada saat tidak menjalankan aplikasi
<img src="img/linux-lts61-idle.png" width="800">

Di bawah ini adalah hasil testing ketika membuka aplikasi youtube dan slims
<img src="img/linux-lts61-using.png" width="800">


#### 4. linux lts66
berikut hasil testing kernel pada saat tidak menjalankan aplikasi
<img src="img/linux-lts66-idle.png" width="800">

Di bawah ini adalah hasil testing ketika membuka aplikasi youtube dan slims
<img src="img/linux-lts66-using.png" width="800">


#### 5. linux mainline
berikut hasil testing kernel pada saat tidak menjalankan aplikasi
<img src="img/linux-mainline-idle.png" width="800">

Di bawah ini adalah hasil testing ketika membuka aplikasi youtube dan slims
<img src="img/linux-mainline-using.png" width="800">


#### 6. linux rt
berikut hasil testing kernel pada saat tidak menjalankan aplikasi
<img src="img/linux-rt-idle.png" width="800">

Di bawah ini adalah hasil testing ketika membuka aplikasi youtube dan slims
<img src="img/linux-rt-using.png" width="800">


#### 7. linux rt lts
berikut hasil testing kernel pada saat tidak menjalankan aplikasi
<img src="img/linux-rt-lts-idle.png" width="800">

Di bawah ini adalah hasil testing ketika membuka aplikasi youtube dan slims
<img src="img/linux-rt-lts-using.png" width="800">


#### 8. linux tachyon
berikut hasil testing kernel pada saat tidak menjalankan aplikasi
<img src="img/linux-tachyon-idle.png" width="800">

Di bawah ini adalah hasil testing ketika membuka aplikasi youtube dan slims
<img src="img/linux-tachyon-using.png" width="800">


#### 9. linux vfio
berikut hasil testing kernel pada saat tidak menjalankan aplikasi
<img src="img/linux-vfio-idle.png" width="800">

Di bawah ini adalah hasil testing ketika membuka aplikasi youtube dan slims
<img src="img/linux-vfio-using.png" width="800">


#### 10. linux vfio lts
berikut hasil testing kernel pada saat tidak menjalankan aplikasi
<img src="img/linux-vfio-lts-idle.png" width="800">

Di bawah ini adalah hasil testing ketika membuka aplikasi youtube dan slims
<img src="img/linux-vfio-lts-using.png" width="800">


#### 11. linux zen
berikut hasil testing kernel pada saat tidak menjalankan aplikasi
<img src="img/linux-zen-idle.png" width="800">

Di bawah ini adalah hasil testing ketika membuka aplikasi youtube dan slims
<img src="img/linux-zen-using.png" width="800">

### desktop environment
untuk riset desktop enviroment team memilih enam kandidat desktop enviroment, kandidat itu diambil dari pertimbangan keringan desktop envoroment tersebut. keenam dari Destop enviroment tersebut diantarnya xfce, lxqt, openbox, fluxbox, mate, dan lxde 
#### lxqt
 | CPU Usage (Saat Pemakaian) | User Experience (UX) |
 |----------------------------|----------------------|
| 50–90%                     | **Tampilan & Desain:**<br>- Kesan visual kuno (default)<br>- Dark mode tersedia<br><br>**Kemudahan Penggunaan:**<br>- Navigasi menu mudah<br>- Pengaturan sistem lengkap<br>- Cocok untuk pemula<br><br>**Responsivitas:**<br>- Mouse & keyboard baik<br>- Animasi UI halus<br><br>**Catatan UX:**<br>- Delay buka aplikasi ±7 detik<br>- Multitasking lancar (5 tab, 6 aplikasi)<br>- Touchpad tap tidak berfungsi|

#### XFCE
| CPU Usage (Saat Pemakaian) | User Experience (UX) |
 |----------------------------|----------------------|
| 3.6–49.7%                     | **Tampilan & Desain:**<br>- Kesan visual: kuno (default)<br>- Dark mode tersedia<br><br>**Kemudahan Penggunaan:**<br>- Navigasi menu mudah<br>- Pengaturan sistem lengkap<br>- Cocok untuk pemula<br><br>**Responsivitas:**<br>- Respons mouse & keyboard baik<br>- Animasi UI halus<br><br>**Catatan UX:**<br>- Sedikit lag saat membuka halaman web berat<br>- Scroll YouTube terasa delay |

 #### Fluxbox
 | CPU Usage (Saat Pemakaian) | User Experience (UX) |
 |----------------------------|----------------------|
|  3.6–49.7%                  | **Tampilan & Desain:**<br>- Kesan visual kaku<br>- Tidak ada dark mode<br><br>**Kemudahan Penggunaan:**<br>- Navigasi menu sulit<br>- Pengaturan sistem minim<br>- Tidak cocok untuk pemula<br><br>**Responsivitas:**<br>- Respons mouse & keyboard baik<br>- Animasi UI halus<br><br>**Catatan UX:**<br>- Sangat ringan<br>- Tidak ada dock bawaan<br>- Akses menu kurang intuitif |

#### LXDE
| CPU Usage (Saat Pemakaian) | User Experience (UX) |
 |----------------------------|----------------------|
| 30–60%                     | **Tampilan & Desain:**<br>- Kesan visual klasik<br>- Konsistensi tema cukup<br>- Dark mode tersedia<br><br>**Kemudahan Penggunaan:**<br>- Navigasi menu mudah<br>- Pengaturan sistem lengkap namun terpisah<br>- Cocok untuk pemula<br><br>**Responsivitas:**<br>- Mouse & keyboard responsif<br>- Animasi UI sedang (kurang halus)<br><br>**Catatan UX:**<br>- Ada jeda saat membuka aplikasi<br>- Scroll YouTube masih lag<br>- Perlu perbaikan untuk penggunaan harian |

#### Openbox
| CPU Usage (Saat Pemakaian) | User Experience (UX) |
 |----------------------------|----------------------|
| 40-67%                    | **Tampilan & Desain:**<br>- osong hanya hitam<br>- Konsistensi tema cukup<br>- Dark mode tersedia<br><br>**Kemudahan Penggunaan:**<br>- Navigasi menu sulitbr>- Pengaturan sistem harus di install manual <br>- Tidak cocok untuk pemula <br><br>**Responsivitas**<br>- Mouse & keyboard responsif<br>- Animasi UI halus (kurang halus)<br><br>**Catatan UX:**<br>- stabil ( di page youtube home delay tidak terlalu parah)<br>- tampilan tidak user friendly<br>- tidak support rounded |

#### Mate
| CPU Usage (Saat Pemakaian) | User Experience (UX) |
 |----------------------------|----------------------|
|82,2-98%| **Tampilan & Desain:**<br>- Kesan visual: kuno (default) m<br>- Konsistensi tema cukup<br>- Dark mode tersedia<br><br>**Kemudahan Penggunaan:**<br>- Navigasi menu mudah br>- Pengaturan sistem lengkap <br>- cocok untuk pemula <br><br>**Responsivitas**<br>- Mouse & keyboard responsif<br>- Animasi UI halus (kurang halus)<br><br>**Catatan UX:**<br>- tampilan mudah di mengerti untuk pemula karena mirip dengan di windows<br>- butuh update tampilan karna tampilan lumayan tua, delay saat scrol yutub<br>- delay saat gonta-ganti tab dan agak sedikit ngelag |

### browser



### Penanganan Error

Dalam pelaksanaan riset, ditemukan beberapa error dan kendala teknis, seperti ketidakstabilan sistem, error aplikasi, maupun hasil pengukuran yang tidak konsisten. Setiap error tidak diabaikan, melainkan dicatat sebagai bagian dari data riset. Tim melakukan analisis penyebab error, kemudian menentukan apakah error tersebut berasal dari faktor sistem, konfigurasi, atau metode pengujian.

Pendekatan ini dilakukan agar hasil riset mencerminkan kondisi nyata di lapangan, bukan hanya kondisi ideal tanpa gangguan.

## Result

### Kernel

| Kernel       | Firefox   | CPU        | RAM       | Delay                                                                                                                                               | Hang                                                              |
| ------------ | --------- | ---------- | --------- | --------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------- |
| lqx          | 30 detik  | 36–89%     | 1,23G     | saat tab yutub dibuka terjadi delay yang cukup lama dan saat kursor digerakan jg terjadi delay                                                      | tidak ada                                                         |
| mainline     | 35 detik  | 36–86%     | 971M      | hanya saat diawal saja selebihnya sudah oke                                                                                                         | tidak ada                                                         |
| vfio         | 37 detik  | 66,2–87,3% | 1,4G      | saat buka firefox terjadi delay yang cukup lama, saat membuka tap yutub terjadi delay, dan juga saat membuka tap baru/gonta-ganti tab terjadi delay | tidak ada                                                         |
| tachyon      | 35 detik  | 36,8–90,1% | 1,4G      | saat buka firefooks terjadi delay yang cukup lama, dan saat searching ada sedikit delay                                                             | tidak ada                                                         |
| linux-git    | 13 detik  | 64–99,1%   | 1,06G     | Ada (saat load video pertama di youtube, setelah load masih ada delay yang terjadi)                                                                 | tidak ada                                                         |
| tkg          | 14 detik  | 46–96%     | 1,07G     | Ada (saat load page youtube video pertama kali ada sedikit lag sekitar 3 detik, setelah play tidak ada delay)                                       | tidak ada                                                         |
| linux-lts61  | 22 detik  | 24–94%     | 1,21G     | Ada (saat load video di youtube)                                                                                                                    | tidak ada                                                         |
| linux lts    | 10 detik  | 43,8%      | 1,216G    | Ada (browser 10–20 detik, buka page berat 4 detik)                                                                                                  | Ada (ketika membuka page berat hang sampai kursor tidak bergerak) |
| linux        | 12 detik  | 43,8%      | 1,18G     | Ada (4 detik)                                                                                                                                       | Ada / Tidak                                                       |
| linux zen    | 12 detik  | 41,7%      | 1,18G     | Ada (4 detik)                                                                                                                                       | Ada / Tidak                                                       |
| linux-rt-lts | 21 detik  | 50–94%     | 1,14G     | Ada (saat load video pertama di youtube, setelah load sudah tidak ada lag lagi)                                                                     | tidak ada                                                         |
| linux-rt     | 12 detik  | 43,8%      | 1,18G     | Ada (4 detik)                                                                                                                                       | Ada / Tidak                                                       |
| lts66        | 24 detik  | 39,8–96%   | 1,11G     | saat buka youtube page delay selama 21 detik dan terjadi delay saat scroll di dalam youtube                                                         | tidak ada                                                         |
| vfio-lts    | 21 detik  | 40–90%     | 1,03G     | delay saat buka page youtube sekitar 8 detik, saat sudah di dalam video lancar                                                                      | tidak ada                                                         |
| **nitrous**  | **gagal** | **gagal**  | **gagal** | **gagal**                                                                                                                                           | **gagal**                                                         |
| **lts515**   | **gagal** | **gagal**  | **gagal** | **gagal**                                                                                                                                           | **gagal**                                                         |
| **lts510**   | **gagal** | **gagal**  | **gagal** | **gagal**                                                                                                                                           | **gagal**                                                         |
| **xanmod** | **gagal** | **gagal** | **gagal** | **gagal** | **gagal** |
| **xanmod-rt** | **gagal** | **gagal** | **gagal** | **gagal** | **gagal** |

## 1. Perbandingan Kecepatan Aplikasi (Firefox)

### Tercepat membuka Firefox

1. **linux lts** – 10 detik
2. **linux / linux zen / linux-rt** – 12 detik
3. **linux-git** – 13 detik
4. **tkg** – 14 detik

### Paling lambat

* **vfio** – 37 detik
* **mainline / tachyon** – 35 detik
* **lqx** – 30 detik

👉 **Catatan:** cepat buka Firefox **tidak selalu berarti respons sistem baik** (contoh: linux lts).

---

## 2. Perbandingan Performa CPU

### CPU Paling Stabil (range tidak ekstrem)

* **mainline** (36–86%)
* **lqx** (36–89%)
* **vfio-lts** (40–90%)
* **linux-rt-lts** (50–94%)

### CPU Paling Agresif / Spike Tinggi

* **linux-git** (hingga 99,1%)
* **tkg** (hingga 96%)
* **lts66** (hingga 96%)

👉 Kernel agresif terasa cepat, tapi **berpotensi bikin lag di hardware lemah**.

---

## 3. Perbandingan Penggunaan RAM

### Paling Hemat RAM

1. **mainline** – 971M
2. **vfio-lts** – 1,03G
3. **linux-git** – 1,06G
4. **tkg** – 1,07G

### Paling Boros RAM

* **vfio / tachyon** – 1,4G
* **lqx** – 1,23G

👉 Untuk RAM 2 GB, **mainline dan vfio-lts paling aman**.

---

## 4. Perbandingan Delay & Respons Sistem

### Delay Paling Ringan / Bisa Ditoleransi

* **mainline** → hanya di awal
* **tkg** → ±3 detik, setelah itu lancar
* **linux-rt-lts** → hanya saat load awal
* **vfio-lts** → ±8 detik, setelah itu lancar

### Delay Berat & Mengganggu

* **lqx** → delay panjang + kursor ikut delay
* **vfio** → delay di hampir semua aktivitas
* **lts66** → delay 21 detik + scroll lag
* **linux lts** → delay browser 10–20 detik

---

## 5. Perbandingan Stabilitas (Hang)

### Paling Stabil (tidak ada hang)

* lqx
* mainline
* vfio
* tachyon
* linux-git
* tkg
* linux-lts61
* linux-rt-lts
* lts66
* vfio-lts

### Ada Risiko Hang

* **linux lts**
* **linux**
* **linux zen**
* **linux-rt**

👉 Kernel non-LTS & non-RT **lebih sering tidak konsisten stabilitasnya**.

---

## 6. Kernel Gagal Total

Tidak lolos pengujian:

* **nitrous**
* **lts515**
* **lts510**
* **xanmod**
* **xanmod-rt**

❌ Tidak layak dipakai di sistem uji ini.

---

## 7. Kesimpulan Akhir (Berdasarkan Data)

### 🔥 Kernel Paling Seimbang (Rekomendasi)

1. **vfio-lts** → RAM hemat, delay ringan, stabil
2. **mainline** → RAM paling irit, delay minimal
3. **tkg** → cepat & responsif setelah load awal

### ⚠️ Cukup Tapi Kurang Nyaman

* lts66
* linux-lts61
* linux-rt-lts

### ❌ Tidak Direkomendasikan

* vfio (non-lts)
* lqx
* linux lts / linux / linux zen / linux-rt
* kernel yang statusnya **gagal**
* 
### Desktop Environment 
Perbandingan Desktop Environment
1. Penggunaan CPU

- Fluxbox memiliki penggunaan CPU paling rendah dan paling stabil, sehingga sangat cocok untuk perangkat dengan spesifikasi sangat terbatas.

- LXDE (Openbox) berada di tingkat menengah, lebih ringan dibanding XFCE dan LXQt, namun masih mengalami lonjakan saat membuka aplikasi.

- XFCE 4.20 (normal & linux-lts) menunjukkan penggunaan CPU cukup tinggi dan fluktuatif, terutama saat browsing dan membuka halaman web berat.

- XFCE (linux-vfio-lts) sedikit lebih efisien dibanding XFCE standar karena batas penggunaan CPU lebih rendah.

- LXQt 2.3 memiliki penggunaan CPU tertinggi, terutama saat multitasking dan membuka aplikasi.

2. Tampilan & Desain

- XFCE dan LXQt menyediakan dark mode dan tampilan yang relatif konsisten, meskipun kesan visual default masih terbilang kuno.

- LXDE memiliki tampilan klasik dengan konsistensi tema cukup baik, namun animasi UI kurang halus.

- Fluxbox paling minim secara visual, tampilan kaku, tanpa dark mode, dan lebih fokus pada efisiensi daripada estetika.

- XFCE (linux-vfio-lts) tampil sangat minimal (bahkan kosong), mengutamakan performa dibanding kenyamanan visual.

3. Kemudahan Penggunaan

- XFCE dan LXQt paling ramah pemula karena navigasi menu mudah dan pengaturan sistem lengkap.

- LXDE masih tergolong mudah digunakan, tetapi pengaturan tersebar dan tidak terpusat.

- Fluxbox dan XFCE (linux-vfio-lts) tidak ramah pemula, karena minim GUI, pengaturan manual, dan navigasi menu kurang intuitif.

4. Responsivitas & Kenyamanan

- Fluxbox sangat responsif untuk mouse dan keyboard, cocok untuk penggunaan ringan tanpa multitasking berat.

- XFCE memberikan animasi paling halus, tetapi mengalami lag saat beban kerja meningkat (web berat, YouTube).

- XFCE (linux-vfio-lts) unggul dalam switching workspace dan kestabilan browsing, meskipun ada kendala perangkat input.

- LXDE cukup responsif, namun animasi terasa kaku dan ada jeda saat membuka aplikasi.

- LXQt responsif saat multitasking, tetapi delay awal membuka aplikasi cukup mengganggu.

5. Kecocokan Penggunaan

- Fluxbox → Server ringan, PC sangat lama, atau pengguna mahir yang mengutamakan performa.

- XFCE → Pengguna umum & pemula yang menginginkan kemudahan dan fitur lengkap.

- XFCE (linux-vfio-lts) → Pengguna lanjutan yang fokus stabilitas dan performa khusus.

- LXDE → Pengguna dengan spesifikasi rendah yang tetap menginginkan antarmuka grafis sederhana.

- LXQt → Pengguna multitasking dengan spesifikasi menengah ke atas.
## Conclusion

### Desktop Environment
Berdasarkan perbandingan penggunaan CPU dan pengalaman pengguna (UX), setiap desktop environment memiliki keunggulan dan keterbatasan yang berbeda.

XFCE 4.20 (baik kernel normal maupun linux-lts) menawarkan pengalaman pengguna paling seimbang. Navigasi mudah, pengaturan sistem lengkap, dan cocok untuk pemula. Namun, penggunaan CPU relatif tinggi dan performa menurun saat membuka halaman web berat atau melakukan scrolling YouTube, terutama di awal pemakaian.

Fluxbox 1.3.7 merupakan desktop environment paling ringan dari sisi penggunaan CPU. Performa sangat responsif dan cocok untuk perangkat dengan spesifikasi sangat rendah. Akan tetapi, dari sisi UX kurang ramah pengguna karena minim fitur, navigasi menu sulit, dan tidak cocok untuk pemula atau penggunaan harian yang membutuhkan kenyamanan.

XFCE 4.20 (linux-vfio-lts) menunjukkan stabilitas performa yang lebih baik dibanding XFCE standar, dengan penggunaan CPU lebih rendah dan browsing lebih stabil. Namun, kekurangan pada fungsionalitas (tampilan kosong, touchpad tidak berfungsi, konfigurasi manual) membuatnya kurang ideal untuk pengguna umum dan lebih cocok untuk pengguna tingkat lanjut.

LXDE (Openbox) berada di posisi tengah antara ringan dan mudah digunakan. Penggunaan CPU lebih rendah dibanding XFCE, navigasi cukup ramah pemula, tetapi animasi kurang halus dan masih terdapat lag saat membuka aplikasi atau scrolling video, sehingga belum optimal untuk penggunaan harian intensif.

LXQt 2.3 menawarkan fitur dan multitasking yang baik, tampilan modern dengan dark mode, serta pengaturan sistem lengkap. Namun, penggunaan CPU cenderung tinggi dan terdapat delay signifikan saat membuka aplikasi, yang mengurangi efisiensi pada perangkat dengan sumber daya terbatas.

- Secara umum, tidak ada desktop environment yang unggul di semua aspek.

- Untuk perangkat sangat low-spec, Fluxbox paling efisien namun mengorbankan kenyamanan.

- Untuk pengguna pemula, XFCE dan LXQt lebih ramah, meski lebih berat.

- Untuk keseimbangan ringan dan usability, LXDE dan XFCE (dengan optimasi) menjadi pilihan kompromi terbaik.
