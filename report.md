# Laporan Hasil Research

## Background

Quinton merpukana riset yang bertujuan untuk pengembangan sistem operasi bagi lembaga GLAM (Gallery, Library, Archives, and Museums). Riset ini bertujuan untuk mencari kernel dan desktop environment yang cocok digunakan bagi perangkat dengan spesifikasi rendah dan waktu produksi yang telah lebih dari 10 tahun. Cakupan penelitian yang mengambil dengan batasan spesifikasi rendah yang telah lebih dari 10 tahun karena tingginya utilitas penggunaan perangkat yang menggunakan spesifikasi rendah dan umur produksi yang lebih dari 10 tahun di perpustakaan. Data tersebut didapatkan dari hasil riset yang bekerja sama dengan HMPS Ilmu Perpustakaan UIN Syarif Hidayatullah Jakarta dari beberapa sampel yang dikumpulkan dari berbagai instansi yang ada di Jakarta.  

## Spesification

Untuk riset ini kami menggunakan perangkat laptop dengan spesifikasi sebagai berikut

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

## Methods

### Pengumpulan Data

1. Mengumpulkan informasi melalui kerjasama dengan organisasi terkait untuk pengumpulan spesifikasi komputer
2. Pengolahan data spesifikasi komputer untuk mendapatkan gambaran umum terkait spesifikasi komputer yang digunakan di perpustakaan
3. Mengumpulkan informasi-informasi kernel yang memungkinkan untuk bisa berjalan secara optimal pada spesifikasi komputer yang didapat
4. Mengumpulkan informasi-informasi desktop environment yang memungkinkan untuk bisa berjalan secara optimal pada spesifikasi komputer yang didapat
5. Mengumpulkan informasi-informasi browser yang memungkinkan untuk bisa berjalan secara optimal pada spesifikasi komputer yang didapat

### Pelaksanaan Eksperimen

1. Melakukan instalasi kernel yang berpotensi kepada sistem uji coba
2. Melakukan instalasi desktop environment yang berpotensi kepada sistem uji coba
3. Melakukan instalasai aplikasi untuk mendukung hasil penelitian
4. Melakukan benchmarking dan pencatatan hasil benchmarking terhadap setiap kernel dan desktop environment
5. Menerapkan sistem ranking untuk menetapkan candidate terbaik

## Result

### Kernel

| Kernel | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | Load Firefox |
| ------ | -------- | -------- | ------------- | ------------- | ------------ |
| vfio    | 26,9%    | 354M     | 66,2–87,3%    | 1,4G          | 37 detik     |

<img src="img/linux-vfio-idle.png" width="800">

> Berikut hasil testing kernel pada saat tidak menjalankan aplikasi  

<img src="img/linux-vfio-using.png" width="800">

### Desktop Enviroment

#### fluxbox 1.2.7
| Desktop Environment | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | UX |
|---------------------|----------|----------|---------------|---------------|----|
| Fluxbox 1.3.7 | 2,6% | 309M | 3,6–49,7% | 887M | Tampilan minimalis dan cenderung kaku; tidak ada dark mode bawaan. Navigasi menu cukup sulit bagi pemula karena berbasis klik kanan tanpa panel modern. Respons mouse dan keyboard baik, sistem terasa ringan dan cepat, namun fitur visual terbatas serta tidak ada dock bawaan. |
- bukti saat idle
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/0a3e873c-d589-4686-bf6a-425e856393af" />

- bukti saat pemakaian
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/2e276cc5-5a57-498e-93a5-a885d7dd54c9" />

  
#### Openbox 3.6.1
| Desktop Environment | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | UX |
|---------------------|----------|----------|---------------|---------------|----|
| Openbox 3.6.1 | 1% | 394M | 40–67% | 1,02G | Tampilan sangat minimalis (default hanya layar hitam) dengan dark mode. Navigasi menu sulit dan pengaturan sistem harus dipasang manual, sehingga tidak ramah pemula. Respons workspace cepat dan animasi halus, namun touchpad untuk klik tidak berfungsi serta tampilan kurang user-friendly tanpa konfigurasi tambahan. |
- bukti saat idle
- <img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/ccd144e0-63b3-4b50-b6cf-a135e6ff814b" />

- bukti saat pemakaian
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/d98d7006-957b-4ffa-b08e-44d8cc0a2003" />


#### lxde 
| Desktop Environment | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | UX |
|---------------------|----------|----------|---------------|---------------|----|
| LXDE 1508 | 2,3% | 482M | 30–60% | 1020M | Tampilan klasik dengan dark mode dan navigasi menu yang mudah, sehingga ramah untuk pemula. Pengaturan sistem cukup lengkap meski tersebar di banyak bagian. Respons mouse dan keyboard baik, switching workspace lancar, namun animasi kurang halus dan ada jeda saat membuka aplikasi serta lag saat scroll YouTube. |
- bukti saat idle
- <img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/16443ce9-0a6f-491b-8116-0b7560a45bf1" />

- bukti saat pemakaian
- <img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/b093f400-7486-45b2-b72c-b9e1c9927e35" />

#### mate
| Desktop Environment | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | UX |
|---------------------|----------|----------|---------------|---------------|----|
| MATE 1.28.2 | 1,9% | 558M | 82,2–98% | 1,11G | Tampilan default terkesan kuno namun mendukung dark mode. Navigasi menu mudah dan pengaturan sistem lengkap, sehingga ramah untuk pemula. Respons mouse dan keyboard baik dengan animasi halus, tetapi terdapat delay saat membuka halaman baru, berpindah tab, dan scroll YouTube. |
- bukti saat idle
- <img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/3eefd623-b037-4d55-9554-82e2d8cfaadd" />
- bukti saat pemakaian
- <img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/65f5a92f-76a4-4794-adbf-85a628137f25" />

#### XFCE
| Desktop Environment | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | UX |
|---------------------|----------|----------|---------------|---------------|----|
| XFCE 4.20 | 2% | 565M | 40–90% | 1,03G | Tampilan default terkesan kuno namun mendukung dark mode. Navigasi menu mudah dan pengaturan sistem lengkap, sehingga ramah untuk pemula. Respons mouse dan keyboard baik dengan animasi halus, serta stabil untuk penggunaan harian, meskipun ada sedikit lag saat membuka halaman baru dan scroll YouTube. |
- bukti saat idle
- <img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/6927ec12-735e-404d-9903-60d731c336d5" />

- bukti saat pemakaian
- <img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/5c349f57-cf2f-4b76-a29b-8a64805b81a1" />

#### icewm
| Desktop Environment | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | UX |
|---------------------|----------|----------|---------------|---------------|----|
| IceWM 4.0.0 | 2,9% | 418M | 36–90% | 1,14G | Tampilan default sangat sederhana dengan taskbar di bawah dan mendukung dark mode. Navigasi menu sedikit sulit bagi pengguna baru meski pengaturan sistem cukup lengkap. Respons mouse dan keyboard baik dengan animasi halus, serta performa stabil, namun tampilan terasa tua dan ada sedikit delay saat scroll YouTube. | 
- bukti saat idle
- <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/92925252-5d5e-4848-8fe7-c3fef5c43d91" />
- bukti saat pemakaian
- <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c0665344-67cf-4536-958b-3efbb34c88b0" />

#### lxqt
| Desktop Environment | CPU Idle | RAM Idle | CPU Pemakaian | RAM Pemakaian | UX |
|---------------------|----------|----------|---------------|---------------|----|
| LXQt 2.3 | 3,9% | 543M | 50–90% | 1,13G | Tampilan default terkesan kuno namun mendukung dark mode. Navigasi menu mudah dan pengaturan sistem lengkap sehingga ramah untuk pemula. Respons mouse dan keyboard baik dengan animasi halus, performa multitasking stabil, namun ada delay saat membuka aplikasi dan scroll YouTube, serta tap touchpad tidak berfungsi. |
- bukti saat idle
<img width="1886" height="979" alt="image" src="https://github.com/user-attachments/assets/eb434311-09d0-462b-8bfa-99ea4a8e95d0" />
- bukti saat pemakaian
<img width="1886" height="979" alt="image" src="https://github.com/user-attachments/assets/3101e88c-20b0-427e-95b4-e62633402681" />

## Conclusion

Berdasarkan hasil riset, dapat disimpulkan bahwa kernel dan desktop environment yang kami pilih berdasarkan hasil sistem ranking 
