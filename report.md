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

Hasil riset menunjukkan perbedaan yang signifikan pada aspek performa, stabilitas, dan pengalaman pengguna berdasarkan skenario pengujian yang diterapkan. Data yang diperoleh memperlihatkan pola penggunaan sumber daya yang konsisten pada kondisi tertentu, serta peningkatan atau penurunan performa ketika sistem berada di bawah beban.

Dari sisi stabilitas, beberapa skenario berjalan tanpa kendala berarti, sementara skenario lain memunculkan error yang berulang. Temuan ini menjadi indikator penting dalam menilai tingkat keandalan objek yang diteliti. Sementara itu, hasil evaluasi user experience menunjukkan bahwa performa teknis tidak selalu berbanding lurus dengan kenyamanan penggunaan.

Secara keseluruhan, data yang dikumpulkan memberikan gambaran menyeluruh mengenai kelebihan, keterbatasan, dan potensi pengembangan lebih lanjut.

## Conclusion

Berdasarkan seluruh rangkaian riset yang telah dilakukan, dapat disimpulkan bahwa pendekatan riset yang terstruktur dan transparan sangat berpengaruh terhadap kualitas hasil yang diperoleh. Pencatatan error sebagai bagian dari data terbukti memberikan nilai tambah dalam memahami kondisi nyata sistem.

Riset ini berhasil mencapai tujuan awal, yaitu menghasilkan data yang objektif dan dapat digunakan sebagai dasar evaluasi serta pengambilan keputusan. Ke depan, riset lanjutan dapat dilakukan dengan memperluas parameter pengujian atau menambahkan variasi skenario agar hasil yang diperoleh semakin komprehensif dan akurat.
