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



### browser



### Penanganan Error

Dalam pelaksanaan riset, ditemukan beberapa error dan kendala teknis, seperti ketidakstabilan sistem, error aplikasi, maupun hasil pengukuran yang tidak konsisten. Setiap error tidak diabaikan, melainkan dicatat sebagai bagian dari data riset. Tim melakukan analisis penyebab error, kemudian menentukan apakah error tersebut berasal dari faktor sistem, konfigurasi, atau metode pengujian.

Pendekatan ini dilakukan agar hasil riset mencerminkan kondisi nyata di lapangan, bukan hanya kondisi ideal tanpa gangguan.

## Result

### kernel
Dari total 19 kernel yang ditesting, terdapat 5 kernel yang dikategorikan sebagai gagal yaitu kernel nitrous, lts515, lts510, xanmod dan xanmod-rt sementara sisanya berhasil terinstall.

Dari 14 total kernel yang sudah terinstall, kernel vfio-lts yang dinilai paling stabil dan yang menjadi pilihan berdasarkan hasil riset melalui CPU Average, penggunaan ram dan peforma ketika membuka beberapa aplikasi seperti youtube dan slims. Hasil riset menunjukan bahwa CPU usage idle dari kernel vfio-lts berada di angka 2$, sementara untuk penggunaan berada di range 40-90%. Kemudian untuk penggunaan ram nya, vfio-lts memakan ram sebesar 565MB untuk idle nya dan 1,03GB untuk pemakaiannya

*riset menggunakan software htop*

Hasil riset menunjukkan perbedaan yang signifikan pada aspek performa, stabilitas, dan pengalaman pengguna berdasarkan skenario pengujian yang diterapkan. Data yang diperoleh memperlihatkan pola penggunaan sumber daya yang konsisten pada kondisi tertentu, serta peningkatan atau penurunan performa ketika sistem berada di bawah beban.

Dari sisi stabilitas, beberapa skenario berjalan tanpa kendala berarti, sementara skenario lain memunculkan error yang berulang. Temuan ini menjadi indikator penting dalam menilai tingkat keandalan objek yang diteliti. Sementara itu, hasil evaluasi user experience menunjukkan bahwa performa teknis tidak selalu berbanding lurus dengan kenyamanan penggunaan.

Secara keseluruhan, data yang dikumpulkan memberikan gambaran menyeluruh mengenai kelebihan, keterbatasan, dan potensi pengembangan lebih lanjut.

## Conclusion

Berdasarkan seluruh rangkaian riset yang telah dilakukan, dapat disimpulkan bahwa pendekatan riset yang terstruktur dan transparan sangat berpengaruh terhadap kualitas hasil yang diperoleh. Pencatatan error sebagai bagian dari data terbukti memberikan nilai tambah dalam memahami kondisi nyata sistem.

Riset ini berhasil mencapai tujuan awal, yaitu menghasilkan data yang objektif dan dapat digunakan sebagai dasar evaluasi serta pengambilan keputusan. Ke depan, riset lanjutan dapat dilakukan dengan memperluas parameter pengujian atau menambahkan variasi skenario agar hasil yang diperoleh semakin komprehensif dan akurat.
