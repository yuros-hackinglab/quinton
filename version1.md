# 1. Latar Belakang

Quinton merpukana riset yang bertujuan untuk pengembangan sistem operasi bagi lembaga GLAM (Gallery, Library, Archives, and Museums). Riset ini bertujuan untuk mencari kernel, desktop environment, dan browser yang cocok digunakan bagi perangkat dengan spesifikasi rendah dan waktu produksi yang telah lebih dari 10 tahun. Cakupan penelitian yang mengambil dengan batasan spesifikasi rendah yang telah lebih dari 10 tahun karena tingginya utilitas penggunaan perangkat yang menggunakan spesifikasi rendah dan umur produksi yang lebih dari 10 tahun di perpustakaan. Data tersebut didapatkan dari hasil riset yang bekerja sama dengan HMPS Ilmu Perpustakaan UIN Syarif Hidayatullah Jakarta dari beberapa sampel yang dikumpulkan dari berbagai instansi yang ada di Jakarta.  

---

# 2. Spesifikasi

Untuk riset ini kami menggunakan perangkat dengan spesifikasi sebagai berikut

| Jenis   | Spesifikasi                                                |
| ------- | --------------------------------------------------------- |
| RAM     | 2 GB DDR3 PC-10600                                        |
| CPU     | AMD E2-1800/E-350 APU (1.0 GHz, 1MB Cache)                |
| Storage | n/a                                                       |
| Grafis   | AMD Radeon HD 7340                                        |
| Layar   | 14 inci, resolusi 1366 x 768 piksel, LED Backlight (16:9) |

Adapun aplikasi yang kami gunakan untuk membantu melakukan riset sebagai berikut

| Aplikasi | Versi                   |
| -------- | ----------------------- |
| SLiMS    | 9.7.2 (Bulian D Roger)  |
| Htop     | 3.4.1                   |

---

# 3. Metode

Dalam riset ini tim menjalankan dua fase riset. Pada riset fase pertama, tim melakukan riset dokumen untuk mengumpulkan data-data yang memungkinkan akan digunakan untuk sistem operasi berbasis GLAM. Setelah fase pertama selesai, tim melaksanakan fase pelaksanaan eksperimen. 

## 3.1. Riset Dokumen dan Survey

1. Mengumpulkan informasi melalui kerjasama dengan organisasi terkait untuk pengumpulan spesifikasi komputer
2. Pengolahan data spesifikasi komputer untuk mendapatkan gambaran umum terkait spesifikasi komputer yang digunakan di perpustakaan
3. Mengumpulkan informasi-informasi kernel yang memungkinkan untuk bisa berjalan secara optimal pada spesifikasi komputer yang didapat
4. Mengumpulkan informasi-informasi desktop environment yang memungkinkan untuk bisa berjalan secara optimal pada spesifikasi komputer yang didapat
5. Mengumpulkan informasi-informasi browser yang memungkinkan untuk bisa berjalan secara optimal pada spesifikasi komputer yang didapat

## 3.2. Pelaksanaan Eksperimen

1. Melakukan instalasi kernel yang berpotensi kepada sistem uji coba
2. Melakukan instalasi desktop environment yang berpotensi kepada sistem uji coba
3. Melakukan instalasai aplikasi untuk mendukung hasil penelitian
4. Melakukan benchmarking dan pencatatan hasil benchmarking terhadap setiap kernel dan desktop environment
5. Menerapkan sistem ranking untuk menetapkan candidate terbaik

---

# 4. Hasil

Bab ini menyajikan hasil dari seluruh rangkaian pengujian dan riset yang telah dilakukan, mencakup evaluasi kernel, browser, serta aspek performa, stabilitas, dan pengalaman pengguna sebagai dasar analisis pengembangan sistem operasi.

## 4.1. Riset Dokumen dan Survey

Tabel berikut menampilkan hasil riset spesifikasi perangkat komputer di berbagai sekolah, perpustakaan, dan institusi pendidikan yang digunakan sebagai dasar analisis kebutuhan serta kompatibilitas dalam prototyping sistem operasi berbasis GLAM.

| Sekolah                        | Sistem Operasi        | Manufacture           | Model                                   | Processor                                                         | Memory  | Graphic                    | VRAM  |
| ------------------------------ | --------------------- | --------------------- | --------------------------------------- | ----------------------------------------------------------------- | ------- | -------------------------- | ----- |
| SD IT Al-Muzammil              | Windows 11 Home       | Lenovo                | 82RJ                                    | 12th Gen Intel(R) Core(TM) i3-1215U (8 CPU), ~1.2GHz              | 8192MB  | Intel(R) UHD Graphics      | 123MB |
| SMA Dharma Karya UT            | Windows 11 Home       | ASUSTeK Computer INC  | ASUS AIO A3202WBA_A3202WBA              | Intel(R) Celeron(R) 7350 (5CPUs), ~1.1GHz                         | 8192M   | Intel(R) UHD Graphics      | 123MB |
| SDN 01 Bintaro                 | Windows 11 Home       | LENOVO                | M42KT36A                                | 12th Gen Intel(R) Core(TM) i5-12400 (12 CPU), ~2.5GHz             | 8192M   | Intel(R) UHD Graphics 730  | 128MB |
| SMKN 22 Jakarta                | Windows 10 Enterprise | ASUS                  | All Series                              | Intel(R) Core(TM) i3-4160 CPU @ 3.60GHz (4 CPUs), ~3.6GHz         | 4096MB  | Microsoft Basic Display    | 0MB   |
| SMKN 22 Jakarta                | Windows 11 Home       | LENOVO                | F0D7000KID                              | Intel(R) Celeron(R) J4005 CPU @ 2.00GHz (2 CPUs), ~2.0GHz         | 4096MB  | Intel(R) UHD Graphics 600  | 512MB |
| Sekolah Maleo                  | Windows 11 Home       | LENOVO                | 12CEA03FID                              | 12th Gen Intel (R) Core(TM) i3-1219U (8 CPUs), ~1.2GHz            | 16384MB | Intel(R) UHD Graphics      | 128MB |
| SMA Negeri 5 Tambun Selatan    | windows 11 home       | HP                    | HP 205 Pro G4 22 All-in-One PC          | AMD Athlon Silver 3050U with Radeon Graphics                      | 4096MB  | AMD Radeon(TM) graphics    | n/a   |
| SMAN 111 jakarta               | Windows 10 Home       | LENOVO                | F0EB00HBID                              | n/a                                                               | 4096MB  | Intel(R) UHD Graphics      | 128MB |
| Al-Ahzar BSD                   | windows 11 pro        | ASUS                  | System Product Name                     | Intel(R) Core(TM) i3-10105 CPU @ 3.70GHz (8 CPUs), ~3.7GHz        | 8192MB  | Intel(R) UHD Graphics 630  | 128MB |
| Perpustakaan Istiqlal          | Windows 10 Pro        | LENOVO                | F0D8001HID                              | n/a                                                               | 4096MB  | AMD Radeon(TM) R4 graphics | 67MB  |
| Fakultas Kedokteran UIN        | Windows 10 Home       | HP                    | HP 200 Pro G4 22 All-in-One PC          | Intel(R) Core(TM) i5-10210U CPU @ 1.60GHz (8 CPUs), ~2.1GHz       | 8192MB  | Intel(R) UHD Graphics      | 128MB |
| Perpustakaan Jakarta Timur     | windows 11 pro        | AXIOO                 | MyPC PRO                                | 11th Gen Intel(R) Core(TM) i5-11400 @ 2.60GHz (12 CPUs), ~2.6GHz  | 8192MB  | Intel(R) UHD Graphics 730  | 128MB |
| Perpustakaan Jakarta Timur     | windows 11 home       | ASUSTeK COMPUTER INC. | ASUS EXPERTCENTER AIO E5402WHA_E5402WHA | 11th Gen Intel(R) Core(TM) i5-11500B @ 3.30GHz (12 CPUs), ~3.3GHz | 8192MB  | Intel(R) UHD Graphics      | 128MB |
| Institut Pariwisata Trisakti   | windows 11 home       | LENOVO                | 12CEA03FID                              | 12th Gen Intel(R) Core(TM) i3-1215U (8 CPUs), ~1.2GHz             | 16384MB | Intel(R) UHD Graphics      | 128MB |
| Perpustakaan Tangerang Selatan | windows 11 home       | ASUSTeK COMPUTER INC. | ASUS EXPERTCENTER AIO E5402WHA_E5402WHA | 11th Gen Intel(R) Core(TM) i5-11500B @ 3.30GHz (12 CPUs), ~3.3GHz | 8192MB  | Intel(R) UHD Graphics      | 128MB |
| Perpustakaan Umum Kota Depok   | windows 11 pro        | HP                    | HP 200 Pro G4 22 All-in-One PC          | Intel(R) Core(TM) i5-10210U @ 1.60 GHz (8 CPUs), ~2.1GHz          | 8192MB  | Intel(R) UHD Graphics      | 128MB |
| SMP Dharma Karya UT            | windows 11 home       | ASUSTeK COMPUTER INC. | ASUS Vivo AIO V222GAR_V222GA            | Intel(R) Celeron(R) J4025 @ 2.00 GHz (2 CPUs), ~2.0 GHz           | 4096MB  | Intel(R) UHD Graphics 600  | 128MB |
| Perpustakaan MI Pembangunan    | windows 11 pro        | Hawlett-Packard       | 20-a210                                 | Intel(R) Core(TM) i3-3240 CPU @ 3.40GHz (4 CPUs), ~3.4GHz         | 6144MB  | Intel(R) UHD Graphics      | 32MB  |

Berdasarkan tabel tersebut data spesifikasi komputer yang digunakan di berbagai sekolah, perpustakaan, dan institusi pendidikan, dengan mayoritas perangkat menggunakan sistem operasi Windows 11 (Home dan Pro) serta sebagian komputer masih menggunakan Windows 10. Produsen yang paling banyak digunakan adalah Lenovo, ASUS, dan HP, didominasi oleh perangkat All-in-One PC. Spesifikasi hardware sangat bervariasi, mulai dari prosesor kelas entry-level seperti Intel Celeron dan AMD Athlon hingga Intel Core i3 dan i5 dari berbagai generasi, dengan kapasitas RAM berkisar antara 4 GB hingga 16 GB. Seluruh perangkat menggunakan grafis terintegrasi (Intel UHD, AMD Radeon, atau Microsoft Basic Display) dengan VRAM relatif kecil.

Tabel berikut menyajikan berbagai varian kernel Linux beserta sumber paketnya, yang digunakan sebagai dasar pengujian stabilitas, performa, dan kompatibilitas prosesor kelas entry-level dalam pengembangan sistem operasi berbasis GLAM.

| Kernel          | Source                                                                      |
| --------------- | --------------------------------------------------------------------------- |
| Lqx             | [link](https://liquorix.net)                                                |                                                                                                     
| Mainline        | [link](https://gitlab.com/chaotic-aur/pkgbuilds/-/tree/main/linux-mainline) |
| Vfio             | [link](https://aur.archlinux.org/linux-vfio.git)                             |
| Tachyon         | [link](https://gitlab.com/chaotic-aur/pkgbuilds/-/tree/main/linux-tachyon)  |
| linux-git       | [link](https://aur.archlinux.org/linux-git.git)                             |
| tkg             | [link](https://github.com/Frogging-Family/linux-tkg)                        |
| linux-lts61     | [link](https://gitlab.com/chaotic-aur/pkgbuilds/-/tree/main/linux-lts61)    |
| linux lts       | [link](https://archlinux.org/packages/core/x86_64/linux-lts/)               |
| linux           | [link](https://archlinux.org/packages/core/x86_64/linux/)                   |
| Linux- zen      | [link](https://archlinux.org/packages/extra/x86_64/linux-zen/)              |
| linux - rt -lts | [link](https://archlinux.org/packages/extra/x86_64/linux-rt-lts/)           |
| linux - rt      | [link](https://archlinux.org/packages/extra/x86_64/linux-rt/)               |
| lts 66          | [link](https://gitlab.com/chaotic-aur/pkgbuilds/-/tree/main/linux-lts66)    |
| vfio-lts         | [link](https://aur.archlinux.org/linux-vfio-lts.git)                         |
| nitrous         | [link](https://gitlab.com/chaotic-aur/pkgbuilds/-/tree/main//linux-nitrous) |
| lts515          | [link](https://aur.archlinux.org/linux-lts515.git)                          |
| lts510          | [link](https://aur.archlinux.org/linux-lts510.git)                          |
| xanmod          | [link](https://aur.archlinux.org/linux-xanmod.git)                          |
| xanmod-rt       | [link](https://gitlab.com/chaotic-aur/pkgbuilds/-/tree/main/linux-xanmod-rt)|

Tabel ini menampilkan daftar berbagai varian kernel Linux yang diuji untuk pengembangan sistem operasi, mencakup kernel stabil (LTS), kernel real-time (RT), kernel optimasi performa (Zen, Tachyon, XFIO), hingga kernel dari repositori pengembangan terbaru (linux-git, tkg, xanmod). Informasi sumber paket disertakan untuk memudahkan akses dan instalasi. Data ini menunjukkan cakupan kernel yang luas, yang memungkinkan evaluasi menyeluruh terhadap stabilitas, kompatibilitas hardware, dan performa sistem operasi berbasis GLAM.

Tabel berikut menyajikan berbagai desktop environment beserta sumber paketnya, yang digunakan untuk pengujian antarmuka, performa, dan efisiensi penggunaan resource dalam pengembangan sistem operasi berbasis GLAM.

| Desktop Enveroment   | Source                                                                    |
| -------              | ------------------------------------------------------------------------- |
| MATE 1.28.2          | [link](https://wiki.archlinux.org/title/MATE)                             |
| Fluxbox 1.3.7        | [link](https://archlinux.org/packages/extra/x86_64/fluxbox/)               |
| Openbox 3.6.1        | [link](https://archlinux.org/packages/extra/x86_64/openbox/)              |
| LXDE 1508            | [link](https://archlinux.org/packages/?sort=&q=lxde&maintainer=&flagged=)  |
| XFCE 4.20            | [link](https://archlinux.org/packages/?sort=&q=xfce&maintainer=&flagged=)  |
| IceWM 4.0.0          | [link](https://archlinux.org/packages/extra/x86_64/icewm/)                |
| LXQt 2.3             | [link](https://archlinux.org/packages/?sort=&q=LXQt+&maintainer=&flagged=) |

Tabel ini menampilkan berbagai desktop environment yang diuji dalam pengembangan sistem operasi, mulai dari yang ringan seperti Fluxbox, Openbox, LXDE, dan IceWM, hingga yang lebih lengkap dan modern seperti MATE, XFCE, dan LXQt. Semua DE memiliki sumber paket yang jelas, memudahkan instalasi dan pengujian. Data ini menunjukkan bahwa setiap DE siap dievaluasi lebih lanjut dari sisi performa, penggunaan resource, dan pengalaman pengguna untuk menentukan antarmuka yang paling sesuai dengan kebutuhan sistem operasi berbasis GLAM.

Tabel berikut menyajikan berbagai browser web beserta sumber paket dan status instalasinya, yang digunakan untuk mengevaluasi kompatibilitas, stabilitas, dan kesiapan aplikasi pada sistem operasi yang dikembangkan.

| Browser  | Source                                                        |
| -------  | --------------------------------------------------------------|
| Firefox  | [link](https://archlinux.org/packages/extra/x86_64/firefox/)   |
| Midori   | [link](https://aur.archlinux.org/midori.git)                  |
| Dillo    | [link](https://aur.archlinux.org/palemoon.git)                |
| Luakit   | [link](https://archlinux.org/packages/extra/x86_64/luakit/)   |
| Netsurf  | [link](https://archlinux.org/packages/extra/x86_64/netsurf/)  |
| Epiphany | [link](https://archlinux.org/packages/extra/x86_64/epiphany/) |

Tabel ini menampilkan daftar browser yang diuji untuk sistem operasi yang dikembangkan beserta sumber paketnya. Browser yang dipilih mencakup opsi populer dan ringan, mulai dari Firefox yang kaya fitur, hingga Dillo, Luakit, Netsurf, dan Epiphany yang lebih ringan. Informasi sumber paket memudahkan instalasi dan pengujian, sekaligus menjadi dasar untuk mengevaluasi kompatibilitas, performa, dan stabilitas masing-masing browser pada sistem operasi.

## 4.2. Pelaksanaan Eksperimen

Pada bagian ini akan melakukan pengujian kernel, desktop environment, dan browser yang akan diterapkan pada sistem operasis berbasis GLAM.

### 4.2.1. Kernel

Pengujian kernel dilihat dari lima instrumen yaitu CPU idle, RAM idle, CPU pemakaian, RAM pemakaian, dan load firefox. 

#### 4.2.1.1. kernel vfio

Pengujian kernel VFIO dilakukan untuk mengevaluasi dukungan virtualisasi, stabilitas sistem, serta kelayakannya sebagai kernel yang digunakan dalam pengembangan dan pengujian sistem operasi berbasis GLAM.

<img src="data/image/linux-vfio-idle.png" width="800">

> Berikut hasil testing kernel pada saat tidak menjalankan aplikasi

<img src="data/image/linux-vfio-pemakaian.png" width="800">

> Di atas adalah hasil testing ketika membuka aplikasi youtube dan slims

| Kernel | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | Load Firefox |
| ------ | -------- | -------- | ------------- | ------------- | ------------ |
| vfio    | 26,9%    | 354M     | 66,2–87,3%    | 1,4G          | 37 detik     |

Penggunaan resource pada kernel VFIO dicatat sedang; saat kondisi idle, CPU digunakan sebesar 26,9% dan RAM sebesar 354 MB, sedangkan saat penggunaan aktif, CPU meningkat menjadi 66,2–87,3% dan RAM menjadi 1,4 GB. Waktu load Firefox tercatat 37 detik, yang menunjukkan bahwa aplikasi dapat dijalankan dengan stabil meskipun beban CPU meningkat secara signifikan. Hasil ini menunjukkan bahwa performa kernel cukup handal, namun manajemen CPU yang baik tetap diperlukan saat menjalankan aplikasi berat.

#### 4.2.1.2. kernel git

Pengujian kernel Git dilakukan untuk mengevaluasi performa, stabilitas, dan kompatibilitas perangkat keras pada versi kernel yang dikembangkan langsung dari repositori sumber, guna menilai kelayakannya sebagai basis sistem operasi berbasis GLAM.

<img src="data/image/linux-git-idle.png" width="800">

> Berikut hasil testing kernel pada saat tidak menjalankan aplikasi

<img src="data/image/linux-git-using.png" width="800">

> Di atas adalah hasil testing ketika membuka aplikasi youtube dan slims

| Kernel | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | Load Firefox |
| ------ | -------- | -------- | ------------- | ------------- | ------------ |
| git    | 1-2,6%    | 576M     | 66,2–99,1%    | 1,08G         | 13 detik     |

Penggunaan resource pada kernel Git dicatat sangat rendah saat idle, dengan CPU 1–2,6% dan RAM 576 MB, sedangkan saat digunakan aktif, CPU meningkat menjadi 66,2–99,1% dan RAM menjadi 1,08 GB. Waktu load Firefox tercatat 13 detik, yang menunjukkan bahwa aplikasi dapat dijalankan dengan cepat dan stabil meskipun beban CPU meningkat secara signifikan saat penggunaan aktif. Hasil ini menegaskan bahwa kernel Git mampu menangani aplikasi dengan efisien, terutama dari sisi waktu respon, namun tetap memerlukan perhatian pada beban CPU tinggi.

#### 4.2.1.3. kernel lqx

Pengujian kernel Lqx dilakukan untuk menilai performa dan stabilitasnya dalam kondisi sistem nyata, serta mengevaluasi kemampuannya dalam mendukung aplikasi dan layanan yang dijalankan pada sistem operasi yang dikembangkan untuk GLAM.

<img src="data/image/linux-lqx-idle.png" width="800">

> Berikut hasil testing kernel pada saat tidak menjalankan aplikasi

<img src="data/image/linux-lqx-using.png" width="800">

> Di atas adalah hasil testing ketika membuka aplikasi youtube dan slims

| Kernel | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | Load Firefox |
| ------ | -------- | -------- | ------------- | ------------- | ------------ |
| lqx    | 1,9%     | 661M     | 36-89%        | 1,23G         | 30 detik     |

Penggunaan resource pada kernel Lqx dicatat rendah saat kondisi idle, dengan CPU sebesar 1,9% dan RAM sebesar 661 MB, sedangkan saat digunakan aktif, CPU meningkat menjadi 36–89% dan RAM menjadi 1,23 GB. Waktu load Firefox tercatat 30 detik, yang menunjukkan bahwa aplikasi dapat dijalankan dengan stabil meskipun terjadi peningkatan signifikan pada penggunaan CPU. Hasil ini menunjukkan bahwa kernel Lqx menawarkan keseimbangan antara efisiensi penggunaan resource saat idle dan kemampuan menangani beban kerja aktif.

#### 4.2.1.4. kernel lts61

Pengujian kernel LTS61 dilakukan untuk mengevaluasi stabilitas jangka panjang, penggunaan resource, dan kompatibilitas perangkat keras, sebagai bagian dari penilaian kelayakan kernel ini untuk pengembangan sistem operasi yang handal berbasis GLAM.

<img src="data/image/linux-lts61-idle.png" width="800">

> Berikut hasil testing kernel pada saat tidak menjalankan aplikasi

<img src="data/image/linux-lts61-using.png" width="800">

> Di atas adalah hasil testing ketika membuka aplikasi youtube dan slims

| Kernel | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | Load Firefox |
| ------ | -------- | -------- | ------------- | ------------- | ------------ |
| lts61  | 2,2-3,8% | 600M     | 24-94%        | 1,21G         | 22 detik     |

Penggunaan resource pada kernel LTS61 dicatat rendah saat idle, dengan CPU 2,2–3,8% dan RAM 600 MB, sedangkan saat digunakan aktif, CPU meningkat menjadi 24–94% dan RAM menjadi 1,21 GB. Waktu load Firefox tercatat 22 detik, yang menunjukkan bahwa aplikasi dapat dijalankan dengan cepat dan stabil meskipun beban CPU meningkat secara signifikan. Hasil ini menunjukkan bahwa kernel LTS61 mampu memberikan efisiensi penggunaan resource yang baik saat idle sekaligus menjaga performa saat beban kerja tinggi.

#### 4.2.1.5. kernel lts66

Pengujian kernel LTS66 dilakukan untuk menilai performa, stabilitas, dan efisiensi penggunaan resource pada lingkungan sistem nyata, sekaligus mengevaluasi kelayakannya sebagai kernel jangka panjang untuk pengembangan sistem operasi berbasis GLAM.

<img src="data/image/linux-lts66-idle.png" width="800">

> Berikut hasil testing kernel pada saat tidak menjalankan aplikasi

<img src="data/image/linux-lts66-using.png" width="800">

> Di atas adalah hasil testing ketika membuka aplikasi youtube dan slims

| Kernel | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | Load Firefox |
| ------ | -------- | -------- | ------------- | ------------- | ------------ |
| lts66  | 1,9%     | 630M     | 39,8-96%      | 1,11G         | 24 detik     |

Penggunaan resource pada kernel LTS66 dicatat rendah saat idle, dengan CPU sebesar 1,9% dan RAM sebesar 630 MB, sedangkan saat digunakan aktif, CPU meningkat menjadi 39,8–96% dan RAM menjadi 1,11 GB. Waktu load Firefox tercatat 24 detik, yang menunjukkan bahwa aplikasi dapat dijalankan dengan stabil meskipun terjadi peningkatan signifikan pada penggunaan CPU. Hasil ini menunjukkan bahwa kernel LTS66 mampu menjaga efisiensi resource saat idle sekaligus mempertahankan performa yang baik saat beban kerja tinggi.

#### 4.2.1.6. kernel mainline

Pengujian kernel Mainline dilakukan untuk mengevaluasi kinerja terbaru dari pengembangan inti Linux, termasuk stabilitas, kompatibilitas perangkat keras, dan kemampuan menjalankan aplikasi secara optimal dalam sistem operasi yang dikembangkan untuk GLAM.

<img src="data/image/linux-mainline-idle.png" width="800">

> Berikut hasil testing kernel pada saat tidak menjalankan aplikasi

<img src="data/image/linux-mainline-using.png" width="800">

> Di atas adalah hasil testing ketika membuka aplikasi youtube dan slims

| Kernel   | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | Load Firefox |
| ------   | -------- | -------- | ------------- | ------------- | ------------ |
| mainline | 1,9%     | 360M     | 36-86%        | 971G          | 35 detik     |

Penggunaan resource pada kernel Mainline dicatat sangat rendah saat idle, dengan CPU 1,9% dan RAM 360 MB, sedangkan saat digunakan aktif, CPU meningkat menjadi 36–86% dan RAM menjadi 971 MB. Waktu load Firefox tercatat 35 detik, yang menunjukkan bahwa aplikasi dapat dijalankan dengan stabil meskipun terjadi peningkatan signifikan pada penggunaan CPU. Hasil ini menunjukkan bahwa kernel Mainline mampu menjaga efisiensi penggunaan resource saat idle sekaligus memberikan performa yang baik saat beban kerja aktif.

#### 4.2.1.7. kernel rt

Pengujian kernel RT dilakukan untuk menilai kemampuan sistem dalam menangani proses real-time, termasuk stabilitas, responsivitas, dan penggunaan resource, sebagai bagian dari evaluasi kesesuaian kernel ini untuk aplikasi yang membutuhkan determinisme tinggi pada sistem operasi berbasis GLAM.

<img src="data/image/linux-rt-idle.png" width="800">

> Berikut hasil testing kernel pada saat tidak menjalankan aplikasi

<img src="data/image/linux-rt-using.png" width="800">

> Di atas adalah hasil testing ketika membuka aplikasi youtube dan slims

| Kernel | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | Load Firefox |
| ------ | -------- | -------- | ------------- | ------------- | ------------ |
| rt     | 5,4%     | 538M     | 43,8%         | 1,18G         | 12 detik     |

Penggunaan resource pada kernel RT dicatat rendah hingga sedang saat idle, dengan CPU sebesar 5,4% dan RAM sebesar 538 MB, sedangkan saat digunakan aktif, CPU tercatat 43,8% dan RAM 1,18 GB. Waktu load Firefox tercatat 12 detik, yang menunjukkan bahwa aplikasi dapat dijalankan dengan cepat dan stabil. Hasil ini menunjukkan bahwa kernel RT mampu memberikan responsivitas yang baik sekaligus menjaga efisiensi penggunaan resource pada sistem operasi.

#### 4.2.1.8. kernel rt-lts

Pengujian kernel RT-LTS dilakukan untuk mengevaluasi kinerja real-time dengan dukungan jangka panjang, menilai stabilitas, responsivitas, dan penggunaan resource, serta menilai kelayakannya sebagai kernel andal untuk aplikasi yang membutuhkan determinisme tinggi pada sistem operasi berbasis GLAM.

<img src="data/image/linux-rt-lts-idle.png" width="800">

> Berikut hasil testing kernel pada saat tidak menjalankan aplikasi

<img src="data/image/linux-rt-lts-using.png" width="800">

> Di atas adalah hasil testing ketika membuka aplikasi youtube dan slims

| Kernel | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | Load Firefox |
| ------ | -------- | -------- | ------------- | ------------- | ------------ |
| rt-lts | 1,9%     | 435M     | 50-94%        | 1,14G         | 21 detik     |

Penggunaan resource pada kernel RT-LTS dicatat sangat rendah saat idle, dengan CPU 1,9% dan RAM 435 MB, sedangkan saat digunakan aktif, CPU meningkat menjadi 50–94% dan RAM menjadi 1,14 GB. Waktu load Firefox tercatat 21 detik, menunjukkan bahwa aplikasi dapat dijalankan dengan stabil meskipun beban CPU meningkat secara signifikan. Hasil ini menegaskan bahwa kernel RT-LTS mampu menjaga efisiensi resource saat idle sekaligus mempertahankan performa yang baik saat sistem bekerja aktif.

#### 4.2.1.9. kernel tachyon

Pengujian kernel Tachyon dilakukan untuk menilai performa tinggi dan optimasi sistem, termasuk stabilitas, efisiensi penggunaan resource, dan kompatibilitas perangkat keras, guna mengevaluasi kelayakannya sebagai kernel yang cepat dan responsif untuk pengembangan sistem operasi berbasis GLAM.

<img src="data/image/linux-tachyon-idle.png" width="800">

> Berikut hasil testing kernel pada saat tidak menjalankan aplikasi

<img src="data/image/linux-tachyon-using.png" width="800">

> Di atas adalah hasil testing ketika membuka aplikasi youtube dan slims

| Kernel | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | Load Firefox |
| ------ | -------- | -------- | ------------- | ------------- | ------------ |
| tachyon| 1,6%     | 323M     | 36,8-90,1%    | 1,4G         | 35 detik     |

Penggunaan resource pada kernel Tachyon dicatat sangat rendah saat idle, dengan CPU 1,6% dan RAM 323 MB, sedangkan saat digunakan aktif, CPU meningkat menjadi 36,8–90,1% dan RAM menjadi 1,4 GB. Waktu load Firefox tercatat 35 detik, menunjukkan bahwa aplikasi dapat dijalankan dengan stabil meskipun beban CPU meningkat secara signifikan. Hasil ini menunjukkan bahwa kernel Tachyon menawarkan efisiensi penggunaan resource yang baik saat idle sekaligus performa yang handal saat beban kerja tinggi.

#### 4.2.1.10. kernel vfio-lts

Pengujian kernel VFIO-LTS dilakukan untuk mengevaluasi stabilitas jangka panjang dan dukungan virtualisasi, termasuk penggunaan resource serta kompatibilitas perangkat keras, sebagai dasar penilaian kelayakan kernel ini dalam pengembangan sistem operasi yang andal.

<img src="data/image/linux-vfio-lts-idle.png" width="800">

> Berikut hasil testing kernel pada saat tidak menjalankan aplikasi

<img src="data/image/linux-vfio-lts-using.png" width="800">

> Di atas adalah hasil testing ketika membuka aplikasi youtube dan slims

| Kernel | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | Load Firefox |
| ------ | -------- | -------- | ------------- | ------------- | ------------ |
| vfio-lts| 2%       | 565M     | 40-90%        | 1,03G         | 21 detik     |

Penggunaan resource pada kernel VFIO-LTS dicatat rendah saat idle, dengan CPU 2% dan RAM 565 MB, sedangkan saat digunakan aktif, CPU meningkat menjadi 40–90% dan RAM menjadi 1,03 GB. Waktu load Firefox tercatat 21 detik, menunjukkan bahwa aplikasi dapat dijalankan dengan stabil meskipun terjadi peningkatan signifikan pada penggunaan CPU. Hasil ini menegaskan bahwa kernel VFIO-LTS mampu menjaga efisiensi resource saat idle sekaligus memberikan performa yang handal saat beban kerja tinggi.

#### 4.2.1.11. kernel zen

Pengujian kernel Zen dilakukan untuk menilai performa dan responsivitas sistem yang dioptimalkan, termasuk penggunaan resource, stabilitas, dan kompatibilitas perangkat keras, sebagai bagian dari evaluasi kernel yang cepat dan efisien untuk pengembangan sistem operasi berbasis GLAM.

<img src="data/image/linux-zen-idle.png" width="800">

> Berikut hasil testing kernel pada saat tidak menjalankan aplikasi

<img src="data/image/linux-zen-using.png" width="800">

> Di atas adalah hasil testing ketika membuka aplikasi youtube dan slims

| Kernel | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | Load Firefox |
| ------ | -------- | -------- | ------------- | ------------- | ------------ |
| zen    | 5,4%     | 538M     | 41,7%         | 1,18G         | 12 detik     |

Pada kernel Zen, kondisi idle ditunjukkan dengan penggunaan CPU sebesar 5,4% dan RAM sebesar 538 MB. Saat sistem berada pada kondisi pemakaian, penggunaan CPU tercatat 41,7% dengan konsumsi RAM meningkat menjadi 1,18 GB. Waktu pemuatan (load) Firefox dicatat selama 12 detik, sehingga dapat disimpulkan bahwa kernel Zen memberikan respons aplikasi yang cepat dengan penggunaan sumber daya yang relatif stabil.

Tabel berikut menyajikan hasil pengujian berbagai kernel Linux sebagai bagian dari proses analisis stabilitas, kompatibilitas perangkat keras, dan kelayakan kernel dalam pengembangan sistem operasi berbasis GLAM.

| Kernel   | Source                                                | Status                                  |
| ------- | --------------------------------------------------------- | --------------------------------------------------------- |
| Lqx               | [link](https://liquorix.net)                                                   | proses instalasi dan booting berhasil dengan baik                                                                                                                   |
| Mainline          | [link](https://gitlab.com/chaotic-aur/pkgbuilds/-/tree/main/linux-mainline)    | proses instalasi dan booting berhasil dengan baik                                                                                                                   |
| Vfio              | [link](https://aur.archlinux.org/linux-vfio.git)                               | proses instalasi dan booting berhasil dengan baik                                                                                                                   |
| Tachyon           | [link](https://gitlab.com/chaotic-aur/pkgbuilds/-/tree/main/linux-tachyon)     | proses instalasi dan booting berhasil dengan baik                                                                                                                   |
| linux-git         | [link](https://aur.archlinux.org/linux-git.git)                                | proses instalasi dan booting berhasil dengan baik                                                                                                                   |
| tkg               | [link](https://github.com/Frogging-Family/linux-tkg)                           | proses instalasi dan booting berhasil namun wireless tidak dapat terdeteksi                                                                                         |
| linux-lts61       | [link](https://gitlab.com/chaotic-aur/pkgbuilds/-/tree/main/linux-lts61)       | proses instalasi dan booting berhasil dengan baik                                                                                                                   |
| linux lts         | [link](https://archlinux.org/packages/core/x86_64/linux-lts/)                  | proses instalasi dan booting berhasil dengan baik                                                                                                                   |
| linux             | [link](https://archlinux.org/packages/core/x86_64/linux/)                      | proses instalasi dan booting berhasil dengan baik                                                                                                                   |
| Linux- zen        | [link](https://archlinux.org/packages/extra/x86_64/linux-zen/)                 | proses instalasi dan booting berhasil dengan baik                                                                                                                   |
| linux - rt -lts   | [link](https://archlinux.org/packages/extra/x86_64/linux-rt-lts/)              | proses instalasi dan booting berhasil dengan baik                                                                                                                   |
| linux - rt        | [link](https://archlinux.org/packages/extra/x86_64/linux-rt/)                  | proses instalasi dan booting berhasil dengan baik                                                                                                                   |
| lts 66            | [link](https://gitlab.com/chaotic-aur/pkgbuilds/-/tree/main/linux-lts66)       | proses instalasi dan booting berhasil dengan baik                                                                                                                   |
| vfio-lts          | [link](https://aur.archlinux.org/linux-vfio-lts.git)                           | proses instalasi dan booting berhasil dengan baik                                                                                                                   |
| nitrous           | [link](https://gitlab.com/chaotic-aur/pkgbuilds/-/tree/main//linux-nitrous)    | proses instalasi berjalan dengan lancar akan tetapi saat melakukan booting terjadi kegagalan, karena saat proses booting terjadi black sreen pada fase booting      |
| lts515            | [link](https://aur.archlinux.org/linux-lts515.git)                             | proses instalasi berjalan dengan lancar akan tetapi saat melakukan booting terjadi kegagalan, karena saat proses booting terjadi stuck pada fase load module        |
| lts510            | [link](https://aur.archlinux.org/linux-lts510.git)                             | proses instalasi berjalan dengan lancar akan tetapi saat melakukan booting terjadi kegagalan, karena saat proses booting terjadi stuck pada fase load module        |
| xanmod            | [link](https://aur.archlinux.org/linux-xanmod.git) | proses instalasi berjalan dengan lancar akan tetapi saat melakukan booting terjadi kegagalan, karena saat proses booting terjadi restart sistem hingga kembali ketampilan grub menu        |
| xanmod-rt         | [link](https://gitlab.com/chaotic-aur/pkgbuilds/-/tree/main/linux-xanmod-rt) | proses instalasi berjalan dengan lancar akan tetapi saat melakukan booting terjadi kegagalan, karena saat proses booting terjadi restart sistem hingga kembali ketampilan grub menu |

Hasil pengujian stabilitas dan kompatibilitas berbagai kernel Linux, di mana sebagian besar kernel berhasil diinstal dan melakukan booting dengan baik sehingga layak dijadikan basis pengembangan. Namun, beberapa kernel mengalami kendala pada tahap booting atau dukungan perangkat keras, seperti kegagalan deteksi wireless dan boot failure, yang menegaskan bahwa pemilihan kernel harus mempertimbangkan stabilitas, kompatibilitas hardware, dan keandalan sistem secara keseluruhan.


---

### 4.2.2. Desktop Enviroment

Subbab ini membahas pengujian berbagai desktop environment (DE) untuk sistem operasi yang dikembangkan, dengan fokus pada efisiensi penggunaan resource, performa, stabilitas, dan pengalaman pengguna, guna menentukan antarmuka yang paling sesuai untuk kebutuhan sistem operasi berbasis GLAM.

#### 4.2.2.1. fluxbox

Pengujian desktop environment Fluxbox dilakukan untuk menilai efisiensi penggunaan resource, performa, dan pengalaman pengguna, serta mengevaluasi kelayakannya sebagai antarmuka ringan pada sistem operasi yang dikembangkan untuk GLAM.

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/0a3e873c-d589-4686-bf6a-425e856393af" />

> bukti saat idle

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/2e276cc5-5a57-498e-93a5-a885d7dd54c9" />

> bukti saat pemakaian

| Desktop Environment | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | UX |
|---------------------|----------|----------|---------------|---------------|----|
| Fluxbox 1.3.7 | 2,6% | 309M | 3,6–49,7% | 887M | Tampilan minimalis dan cenderung kaku; tidak ada dark mode bawaan. Navigasi menu cukup sulit bagi pemula karena berbasis klik kanan tanpa panel modern. Respons mouse dan keyboard baik, sistem terasa ringan dan cepat, namun fitur visual terbatas serta tidak ada dock bawaan. |

Pada Fluxbox 1.3.7, kondisi idle ditunjukkan oleh penggunaan CPU sebesar 2,6% dan RAM 309 MB. Saat pemakaian, penggunaan CPU berada pada rentang 3,6–49,7% dengan konsumsi RAM meningkat menjadi 887 MB. Dari sisi UX, tampilan disajikan secara minimalis dan kaku, tanpa dukungan dark mode bawaan. Navigasi dianggap kurang ramah bagi pemula karena bergantung pada menu klik kanan dan tidak dilengkapi panel modern. Meskipun demikian, respons mouse dan keyboard dirasakan baik, sistem berjalan ringan dan cepat, namun dengan keterbatasan fitur visual serta ketiadaan dock bawaan.
  
#### 4.2.2.2. Openbox

Pengujian desktop environment Openbox dilakukan untuk mengevaluasi performa, penggunaan resource, dan pengalaman pengguna, serta menilai kecocokannya sebagai antarmuka ringan dan responsif pada sistem operasi yang dikembangkan untuk GLAM.

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/ccd144e0-63b3-4b50-b6cf-a135e6ff814b" />

> bukti saat idle

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/d98d7006-957b-4ffa-b08e-44d8cc0a2003" />

> bukti saat pemakaian

| Desktop Environment | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | UX |
|---------------------|----------|----------|---------------|---------------|----|
| Openbox 3.6.1 | 1% | 394M | 40–67% | 1,02G | Tampilan sangat minimalis (default hanya layar hitam) dengan dark mode. Navigasi menu sulit dan pengaturan sistem harus dipasang manual, sehingga tidak ramah pemula. Respons workspace cepat dan animasi halus, namun touchpad untuk klik tidak berfungsi serta tampilan kurang user-friendly tanpa konfigurasi tambahan. |

Pada Openbox 3.6.1, penggunaan CPU saat idle tercatat sebesar 1% dengan konsumsi RAM 394 MB, sedangkan pada kondisi pemakaian penggunaan CPU berada pada kisaran 40–67% dan RAM meningkat hingga 1,02 GB; dari sisi pengalaman pengguna, tampilan yang disajikan bersifat sangat minimalis dengan kondisi bawaan berupa layar hitam serta dukungan dark mode, navigasi menu dinilai cukup sulit dan pengaturan sistem harus dilakukan secara manual sehingga kurang ramah bagi pemula, meskipun respons perpindahan workspace terasa cepat dan animasi berjalan halus, fungsi touchpad untuk klik dilaporkan tidak berfungsi optimal serta tampilan keseluruhan kurang user-friendly tanpa konfigurasi tambahan.

#### 4.2.2.3. lxde 

Pengujian desktop environment LXDE dilakukan untuk menilai efisiensi penggunaan resource, performa sistem, dan pengalaman pengguna, serta mengevaluasi kelayakannya sebagai antarmuka ringan yang cocok untuk sistem operasi berbasis GLAM dengan spesifikasi terbatas.

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/16443ce9-0a6f-491b-8116-0b7560a45bf1" />

> bukti saat idle

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/b093f400-7486-45b2-b72c-b9e1c9927e35" />

> bukti saat pemakaian

| Desktop Environment | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | UX |
|---------------------|----------|----------|---------------|---------------|----|
| LXDE 1508 | 2,3% | 482M | 30–60% | 1020M | Tampilan klasik dengan dark mode dan navigasi menu yang mudah, sehingga ramah untuk pemula. Pengaturan sistem cukup lengkap meski tersebar di banyak bagian. Respons mouse dan keyboard baik, switching workspace lancar, namun animasi kurang halus dan ada jeda saat membuka aplikasi serta lag saat scroll YouTube. |

Pada LXDE 1508, penggunaan CPU saat idle berada pada kisaran 2,3% dengan konsumsi RAM sebesar 482 MB, sedangkan pada kondisi pemakaian CPU tercatat 30–60% dan RAM meningkat hingga 1.020 MB; dari sisi pengalaman pengguna, tampilan yang disajikan bersifat klasik dengan dukungan dark mode serta navigasi menu yang mudah dipahami sehingga dinilai ramah bagi pemula, pengaturan sistem tersedia cukup lengkap meskipun tersebar di beberapa bagian, respons mouse dan keyboard berjalan baik serta perpindahan workspace terasa lancar, namun animasi dinilai kurang halus dan ditemukan jeda saat membuka aplikasi serta lag ketika melakukan scroll pada YouTube.

#### 4.2.2.4. mate

Pengujian desktop environment MATE dilakukan untuk mengevaluasi performa, penggunaan resource, dan pengalaman pengguna, serta menilai kecocokannya sebagai antarmuka yang stabil dan fungsional pada sistem operasi berbasis GLAM yang dikembangkan.

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/3eefd623-b037-4d55-9554-82e2d8cfaadd" />

> bukti saat idle

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/65f5a92f-76a4-4794-adbf-85a628137f25" />

> bukti saat pemakaian

| Desktop Environment | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | UX |
|---------------------|----------|----------|---------------|---------------|----|
| MATE 1.28.2 | 1,9% | 558M | 82,2–98% | 1,11G | Tampilan default terkesan kuno namun mendukung dark mode. Navigasi menu mudah dan pengaturan sistem lengkap, sehingga ramah untuk pemula. Respons mouse dan keyboard baik dengan animasi halus, tetapi terdapat delay saat membuka halaman baru, berpindah tab, dan scroll YouTube. |

Pada MATE 1.28.2, penggunaan CPU saat kondisi idle tercatat sebesar 1,9% dengan konsumsi RAM 558 MB, sementara pada kondisi pemakaian CPU meningkat pada kisaran 82,2–98% dan penggunaan RAM mencapai 1,11 GB; dari sisi pengalaman pengguna, tampilan default dinilai terkesan kuno namun telah mendukung dark mode, navigasi menu dapat digunakan dengan mudah dan pengaturan sistem tersedia lengkap sehingga dinilai ramah bagi pemula, respons mouse dan keyboard berjalan baik dengan animasi yang relatif halus, meskipun masih ditemukan delay saat membuka halaman baru, berpindah tab, serta ketika melakukan scroll pada YouTube.

#### 4.2.2.5. XFCE

Pengujian desktop environment XFCE dilakukan untuk menilai efisiensi penggunaan resource, performa, dan pengalaman pengguna, serta mengevaluasi kelayakannya sebagai antarmuka ringan dan stabil yang sesuai untuk sistem operasi berbasis GLAM dengan fokus pada kecepatan dan responsivitas.

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/6927ec12-735e-404d-9903-60d731c336d5" />

> bukti saat idle

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/5c349f57-cf2f-4b76-a29b-8a64805b81a1" />

> bukti saat pemakaian

| Desktop Environment | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | UX |
|---------------------|----------|----------|---------------|---------------|----|
| XFCE 4.20 | 2% | 565M | 40–90% | 1,03G | Tampilan default terkesan kuno namun mendukung dark mode. Navigasi menu mudah dan pengaturan sistem lengkap, sehingga ramah untuk pemula. Respons mouse dan keyboard baik dengan animasi halus, serta stabil untuk penggunaan harian, meskipun ada sedikit lag saat membuka halaman baru dan scroll YouTube. |

Pada XFCE 4.20, penggunaan CPU pada kondisi idle tercatat sebesar 2% dengan konsumsi RAM 565 MB, sedangkan saat pemakaian CPU berada pada kisaran 40–90% dengan penggunaan RAM mencapai 1,03 GB; dari sisi pengalaman pengguna, tampilan default dinilai terkesan kuno namun telah mendukung dark mode, navigasi menu dapat digunakan dengan mudah dan pengaturan sistem tersedia lengkap sehingga ramah bagi pemula, respons mouse dan keyboard berjalan baik dengan animasi yang halus serta dinilai stabil untuk penggunaan harian, meskipun masih ditemukan sedikit lag saat membuka halaman baru dan melakukan scroll pada YouTube.

#### 4.2.2.6. icewm

Pengujian desktop environment IceWM dilakukan untuk mengevaluasi performa, penggunaan resource, dan pengalaman pengguna, serta menilai kelayakannya sebagai antarmuka ringan dan sederhana yang mendukung sistem operasi berbasis GLAM dengan spesifikasi terbatas.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/92925252-5d5e-4848-8fe7-c3fef5c43d91" />

> bukti saat idle

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c0665344-67cf-4536-958b-3efbb34c88b0" />

> bukti saat pemakaian

| Desktop Environment | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | UX |
|---------------------|----------|----------|---------------|---------------|----|
| IceWM 4.0.0 | 2,9% | 418M | 36–90% | 1,14G | Tampilan default sangat sederhana dengan taskbar di bawah dan mendukung dark mode. Navigasi menu sedikit sulit bagi pengguna baru meski pengaturan sistem cukup lengkap. Respons mouse dan keyboard baik dengan animasi halus, serta performa stabil, namun tampilan terasa tua dan ada sedikit delay saat scroll YouTube. | 

Pada IceWM 4.0.0, penggunaan CPU pada kondisi idle berada di angka 2,9% dengan konsumsi RAM 418 MB, sedangkan saat pemakaian CPU tercatat pada kisaran 36–90% dengan penggunaan RAM mencapai 1,14 GB; dari sisi pengalaman pengguna, tampilan default dinilai sangat sederhana dengan taskbar di bagian bawah serta telah mendukung dark mode, navigasi menu dirasakan sedikit sulit bagi pengguna baru meskipun pengaturan sistem tergolong cukup lengkap, respons mouse dan keyboard berjalan baik dengan animasi halus dan performa yang stabil, namun tampilan masih terasa tua serta ditemukan sedikit delay saat melakukan scroll pada YouTube.

#### 4.2.2.7. lxqt

Pengujian desktop environment LXQt dilakukan untuk menilai efisiensi penggunaan resource, performa, dan pengalaman pengguna, serta mengevaluasi kelayakannya sebagai antarmuka modern yang ringan dan responsif untuk sistem operasi berbasis GLAM yang dikembangkan.

<img width="1886" height="979" alt="image" src="https://github.com/user-attachments/assets/eb434311-09d0-462b-8bfa-99ea4a8e95d0" />

> bukti saat idle

<img width="1886" height="979" alt="image" src="https://github.com/user-attachments/assets/3101e88c-20b0-427e-95b4-e62633402681" />

> bukti saat pemakaian

| Desktop Environment | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | UX |
|---------------------|----------|----------|---------------|---------------|----|
| LXQt 2.3 | 3,9% | 543M | 50–90% | 1,13G | Tampilan default terkesan kuno namun mendukung dark mode. Navigasi menu mudah dan pengaturan sistem lengkap sehingga ramah untuk pemula. Respons mouse dan keyboard baik dengan animasi halus, performa multitasking stabil, namun ada delay saat membuka aplikasi dan scroll YouTube, serta tap touchpad tidak berfungsi. |

Pada LXQt 2.3, penggunaan CPU pada kondisi idle tercatat sebesar 3,9% dengan konsumsi RAM 543 MB, sedangkan saat pemakaian CPU berada pada kisaran 50–90% dengan penggunaan RAM mencapai 1,13 GB; dari sisi pengalaman pengguna, tampilan default dinilai terkesan kuno namun telah mendukung dark mode, navigasi menu dinilai mudah dengan pengaturan sistem yang lengkap sehingga relatif ramah bagi pemula, respons mouse dan keyboard berjalan baik dengan animasi halus serta performa multitasking yang stabil, namun masih ditemukan delay saat membuka aplikasi dan melakukan scroll pada YouTube, serta fitur tap touchpad tidak berfungsi.

Tabel berikut menyajikan hasil pengujian instalasi berbagai desktop environment pada sistem operasi yang dikembangkan, mencakup versi, sumber paket, serta status keberhasilan instalasi sebagai dasar evaluasi antarmuka dan performa sistem.

| Desktop Enveroment   | Source                                                | Status                              |
| ------- | --------------------------------------------------------- |--------------------------------------------------------- |
| MATE 1.28.2    | [link](https://wiki.archlinux.org/title/MATE)                                 | Berhasil |
| Fluxbox 1.3.7  | [link](https://archlinux.org/packages/extra/x86_64/fluxbox/)                  | Berhasil |
| Openbox 3.6.1  | [link](https://archlinux.org/packages/extra/x86_64/openbox/)                  | Berhasil |
| LXDE 1508      | [link](https://archlinux.org/packages/?sort=&q=lxde&maintainer=&flagged=)     | Berhasil |
| XFCE 4.20      | [link](https://archlinux.org/packages/?sort=&q=xfce&maintainer=&flagged=)     | Berhasil |
| IceWM 4.0.0    | [link](https://archlinux.org/packages/extra/x86_64/icewm/)                    | Berhasil |
| LXQt 2.3       | [link](https://archlinux.org/packages/?sort=&q=LXQt+&maintainer=&flagged=)    | Berhasil |

Tabel ini menunjukkan bahwa semua desktop environment yang diuji — MATE, Fluxbox, Openbox, LXDE, XFCE, IceWM, dan LXQt — berhasil diinstal dengan baik. Hal ini menandakan bahwa versi-versi yang digunakan kompatibel dengan sistem operasi yang dikembangkan, dan siap untuk diuji lebih lanjut dari sisi performa, penggunaan resource, serta pengalaman pengguna. Dengan keberhasilan instalasi ini, setiap DE dapat dievaluasi untuk menentukan antarmuka yang paling ringan, responsif, dan sesuai kebutuhan target sistem operasi berbasis GLAM.

---

### 4.2.3. Browser

Subbab ini menyajikan hasil pengujian berbagai browser web pada sistem operasi yang dikembangkan, meliputi performa, penggunaan resource, stabilitas, dan pengalaman pengguna, sebagai dasar pemilihan browser yang paling optimal untuk lingkungan sistem operasi berbasis GLAM.

#### 4.2.3.1. falcon

Pengujian browser Falcon dilakukan untuk menilai performa, stabilitas, dan pengalaman pengguna (UX) sebagai kandidat browser pada sistem operasi yang dikembangkan. Pengujian performa dilakukan pada dua kondisi, yaitu saat idle (browser terbuka tanpa tab aktif) dan saat digunakan (beberapa tab aktif seperti SLiMS, Canva, dan YouTube).

| Resource | Nilai |
|--------|------|
| CPU Usage | 4,5 % |
| RAM Usage | 516 M |

Hasil ini menunjukkan bahwa Falcon memiliki konsumsi resource yang relatif rendah saat tidak digunakan secara aktif.

<img width="1896" height="999" alt="Image" src="https://github.com/user-attachments/assets/326c12f0-6678-4536-a3fa-f2bc5075407e" />

> tampilan htop pemakaian resource saat idle

| Resource | Nilai |
|--------|------|
| CPU Usage | 81 % |
| RAM Usage | 820 M |

Pada saat digunakan dengan beberapa tab aktif, terjadi peningkatan signifikan pada penggunaan CPU dan RAM, yang mengindikasikan beban kerja cukup tinggi terhadap sistem.

<img width="1890" height="1006" alt="Image" src="https://github.com/user-attachments/assets/3a304c06-775a-4ad2-ad13-3eab3ab5e2f6" />

> tampilan htop pemakaian resource saat sedang digunakan

| browser | crash | lag | memory leak |
|---------|------|-------|------------|
| falcon  | yes   | yes    | no       |

Berdasarkan hasil pengujian, Falcon mengalami crash dan lag saat digunakan, namun tidak ditemukan indikasi memory leak.

| antarmuka & design | kemudahan | responsivitas |
|--------------------|-----------|---------------|
| buruk | baik | baik |

Secara keseluruhan, Falcon cukup mudah digunakan dan responsif, namun memiliki kekurangan pada aspek visual dan stabilitas saat penggunaan intensif.

---

#### 4.2.3.2. dillo

Pengujian browser Falcon dilakukan untuk menilai performa, stabilitas, dan pengalaman pengguna (UX) sebagai kandidat browser pada sistem operasi yang dikembangkan. Pengujian browser Dillo dilakukan untuk mengevaluasi efisiensi penggunaan resource, stabilitas, dan pengalaman pengguna (UX) dalam konteks pengembangan sistem operasi.

| Resource | Nilai |
|--------|------|
| CPU Usage | 2.6-5% |
| RAM Usage | 239M |

Hasil pengujian menunjukkan bahwa Dillo memiliki konsumsi resource yang sangat rendah saat idle, menjadikannya efisien untuk sistem dengan spesifikasi terbatas.

<img width="1895" height="989" alt="Image" src="https://github.com/user-attachments/assets/a81ac30c-e370-444e-882d-877e155c32c3" />

| Resource | Nilai |
|--------|------|
| CPU Usage | 18 % |
| RAM Usage | 381 M |

Pada saat digunakan, Dillo tetap menunjukkan penggunaan CPU dan RAM yang relatif rendah dibandingkan browser lain, menandakan performa yang ringan dari sisi resource.

<img width="1887" height="953" alt="Image" src="https://github.com/user-attachments/assets/97bb2cb0-efb6-40f7-bb8a-c8dfffb68434" />

> tampilan htop pemakaian resource saat sedang digunakan


| browser | crash | lag | memory leak |
|---------|------|-------|------------|
| dilo    | yes  | yes   | no         |

Berdasarkan hasil pengujian, Dillo mengalami crash dan lag saat penggunaan, namun tidak ditemukan indikasi memory leak. Hal ini menunjukkan bahwa meskipun ringan, stabilitas aplikasi masih menjadi kendala.

| antarmuka & design | kemudahan | responsivitas |
|--------------------|-----------|---------------|
| buruk | sangat buruk | baik |

Secara keseluruhan, Dillo unggul dalam efisiensi resource, namun memiliki keterbatasan signifikan pada aspek pengalaman pengguna dan stabilitas, sehingga perlu dipertimbangkan kembali untuk penggunaan umum pada sistem operasi yang dikembangkan.

---

#### 4.2.3.3. firefox

Pengujian browser Firefox dilakukan untuk menilai performa, stabilitas, dan pengalaman pengguna (UX) sebagai browser umum pada sistem operasi yang dikembangkan. Pengujian dilakukan pada kondisi idle (browser terbuka tanpa tab aktif) dan saat digunakan dengan beberapa tab aktif seperti SLiMS, Canva, dan YouTube.

| Resource | Nilai |
|--------|------|
| CPU Usage | 5-22% |
| RAM Usage | 757M |

Hasil ini menunjukkan bahwa Firefox memiliki konsumsi resource yang relatif tinggi meskipun dalam kondisi idle, terutama pada penggunaan RAM.

<img width="1893" height="1000" alt="Image" src="https://github.com/user-attachments/assets/eb560339-4eaa-4b89-a76e-e7058aefeadc" />

> tampilan htop pemakaian resource saat idle

| Resource | Nilai |
|--------|------|
| CPU Usage | 95 % |
| RAM Usage | 1030 M |

Saat digunakan dengan beberapa tab aktif, Firefox menunjukkan peningkatan penggunaan resource yang signifikan, khususnya pada CPU dan RAM, yang menandakan beban sistem cukup besar.

<img width="1885" height="993" alt="Image" src="https://github.com/user-attachments/assets/9751430b-8dba-4e10-b472-d4e7ff147cd0" />

> tampilan htop pemakaian resource saat sedang digunakan

| browser | crash | lag | memory leak |
|---------|------|-------|------------|
| firefox | no   | yes   | no         |

Berdasarkan hasil pengujian, Firefox tidak mengalami crash dan tidak menunjukkan indikasi memory leak, namun terjadi lag saat penggunaan intensif. Hal ini menunjukkan stabilitas aplikasi yang baik, meskipun performa dapat menurun pada kondisi beban tinggi.


| antarmuka & design | kemudahan | responsivitas |
|--------------------|-----------|---------------|
| sangat baik | baik | sangat baik |

Secara keseluruhan, Firefox unggul pada aspek pengalaman pengguna dan stabilitas, namun memiliki konsumsi resource yang tinggi, sehingga perlu dipertimbangkan dalam pengembangan sistem operasi yang menargetkan perangkat dengan spesifikasi terbatas.

---

#### 4.2.3.4. Epiphany

Pengujian browser Epiphany dilakukan untuk menilai performa, stabilitas, dan pengalaman pengguna (UX) sebagai bagian dari evaluasi browser pada sistem operasi yang dikembangkan. Pengujian performa dilakukan pada kondisi idle dan saat digunakan dengan beberapa tab aktif seperti SLiMS, Canva, dan YouTube.

| Resource | Nilai |
|--------|------|
| CPU Usage | 6% |
| RAM Usage | 532M |

Hasil ini menunjukkan bahwa Epiphany memiliki penggunaan resource yang relatif sedang pada kondisi idle.

<img width="1886" height="979" alt="Image" src="https://github.com/user-attachments/assets/3054ff10-7a60-48d0-9f1d-a80228166bf4" />

> tampilan htop pemakaian resource saat idle

| Resource | Nilai |
|--------|------|
| CPU Usage | 98 % |
| RAM Usage | 881 M |

Pada saat digunakan, terjadi peningkatan penggunaan CPU yang sangat tinggi, menunjukkan beban sistem yang berat meskipun penggunaan RAM masih berada pada tingkat menengah.

<img width="1886" height="979" alt="Image" src="https://github.com/user-attachments/assets/4e21427c-3394-4429-a78d-8bb10d6c20c8" />

> tampilan htop pemakaian resource saat sedang digunakan

| browser | crash | lag | memory leak |
|---------|------|-------|------------|
| epiphany | yes   | yes   | no         |

Berdasarkan hasil pengujian, Epiphany mengalami crash dan lag saat digunakan, namun tidak ditemukan indikasi memory leak. Hal ini menunjukkan bahwa stabilitas aplikasi masih perlu ditingkatkan meskipun manajemen memori tergolong baik.

| antarmuka & design | kemudahan | responsivitas |
|--------------------|-----------|---------------|
| sangat baik | sangat baik | baik |

Secara keseluruhan, Epiphany menawarkan pengalaman pengguna yang baik dari sisi tampilan dan kemudahan, namun memiliki keterbatasan pada aspek performa dan stabilitas saat digunakan secara intensif.

Tabel berikut menampilkan hasil pengujian instalasi dan ketersediaan berbagai browser web yang digunakan sebagai bagian dari evaluasi kompatibilitas aplikasi pada lingkungan sistem operasi berbasis GLAM.

| Browser  | Source                                                        | Status                       |
| -------  | --------------------------------------------------------------| ---------------------------- |
| Firefox  | [link](https://archlinux.org/packages/extra/x86_64/firefox/)   | berhasil                     |
| Midori   | [link](https://aur.archlinux.org/midori.git)                  | gagal saat melakukan makepkg |
| Dillo    | [link](https://aur.archlinux.org/palemoon.git)                | berhasil                     | 
| Luakit   | [link](https://archlinux.org/packages/extra/x86_64/luakit/)   | berhasil                     |
| Netsurf  | [link](https://archlinux.org/packages/extra/x86_64/netsurf/)  | berhasil                     |
| Epiphany | [link](https://archlinux.org/packages/extra/x86_64/epiphany/) | berhasil                     |

Tabel ini menunjukkan hasil pengujian browser pada sistem operasi yang dikembangkan, di mana sebagian besar browser berhasil diinstal dengan baik, sementara Midori mengalami kegagalan pada proses makepkg, menandakan adanya kendala kompatibilitas atau dependensi.

---

# 5. Kesimpulan

- Berdasarkan data sampel spesifikasi yang dikumpulkan maka dapat disimpulkan spesifikasi komputer berada pada level low sampai dengan mid end
- Rekomendasi kernel untuk sistem operasi berbasis GLAM adalah linux-zen, linux-vfio dan linux-vfio-lts
- Rekomendasi desktop environment untuk sistem operasi berbasis GLAM adalah Gnome dan Openbox
- Rekomendasi browser untuk sistem operasi berbasis GLAM adalah Firefox dan Epiphany

# 6. Referensi
