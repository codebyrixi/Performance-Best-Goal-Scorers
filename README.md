# Performance of the Best Goal Scorers in International Football
Proyek ini menganalisis performa pencetak gol terbaik dalam sepak bola internasional, dengan fokus pada efisiensi, tren historis, dan kontribusi negara. Hasilnya menunjukkan dominasi konfederasi tertentu dan kontribusi signifikan pemain dalam kesuksesan tim nasional mereka.

## Daftar Isi
- Latar Belakang
- Data Cleaning and Preprocessing
- Visualisasi Data
- Kesimpulan

## Bagian 1: Gambaran Umum
**Latar Belakang**<br>
Sepak bola internasional adalah salah satu olahraga paling populer di dunia, dengan pemain-pemain legendaris yang meninggalkan jejak melalui pencapaian luar biasa, seperti mencetak lebih dari 50 gol internasional. Rekor ini mencerminkan tidak hanya kehebatan individu, tetapi juga kontribusi mereka terhadap kesuksesan tim nasional mereka. Dengan menganalisis performa para pemain ini, kita dapat memperoleh wawasan yang berharga tentang pola pencapaian, evolusi performa, serta dampak mereka terhadap perkembangan sepak bola global.

**Tujuan**<br>
Berikut adalah tujuan dari penelitian ini:
1. Mengidentifikasi pemain dengan rasio gol per pertandingan tertinggi dalam sejarah sepak bola internasional.
2. Menganalisis kontribusi negara-negara terhadap daftar pemain pencetak gol terbanyak dan hubungannya dengan perkembangan sepak bola di wilayah tersebut.
3. Mengungkap tren historis pencapaian gol internasional, termasuk perubahan pola pencapaian dari era ke era.
4. Memberikan wawasan yang relevan bagi peneliti, analis, dan penggemar sepak bola mengenai dampak pencetak gol terhadap kesuksesan tim nasional.

**Metriks Bisnis**<br>
Berikut adalah metriks bisnis dari penelitian ini:
1. _Goals per Match (GPM)_: Mengukur efisiensi pemain dalam mencetak gol per pertandingan internasional.
2._ Total Goals Scored_: Jumlah keseluruhan gol yang mencerminkan performa dan kontribusi pemain.
3. _Career Longevity_: Rentang waktu karir internasional yang menunjukkan konsistensi performa pemain.
4. _Nation's Representation_: Jumlah pemain dari masing-masing negara, mencerminkan tingkat pengembangan dan dominasi sepak bola negara tersebut.
5. _Timeline of 50th Goal Achievement_: Waktu yang diperlukan pemain untuk mencapai milestone 50 gol, sebagai indikator percepatan performa.

**Deskripsi Fitur**<br>
| Fitur | Deskripsi |
|:---:|:---:|
| `Rank` | Peringkat pemain berdasarkan total gol internasional. |
| `Player` | Nama Pemain |
| `Nation` | Negara yang diwakili pemain. |
| `Confederation` | Konfederasi sepak bola pemain. |
| `Goals` | Jumlah total gol. |
| `Caps` | Jumlah pertandingan internasional. |
| `Goals per Match` | Rata-rata gol per pertandingan. |
| `Career Span Begin` | Waktu awal berkarir. |
| `Career Span Last` | Waktu karirnya berakhir. |
| `Date of 50th Goal` | Tanggal mencapai 50 gol. |

## Bagian 2: Data Cleaning and Preprocessing
Dari tabel dibawah, hanya ada dua hal yang dilakukan pada tahapan ini, yaitu _handling missing value_ dan _handling outliers_. Namun _handling missing value_ tidak dilakukan karena jika dilihat pada tabel sample sebelumnya, terlihat bahwa beberapa pemain memiliki _career span begin_ yang tidak diketahui. Oleh karena itu, hal ini masih dapat diwajari dan tidak seharusnya dihapus. Oleh karena itu, pada tahapan ini hanya akan dilakukan penanganan _outlier_ (pencilan).
| Jenis Anomali Data | Temuan | Jenis Anomali Data | Temuan |
|---|---|---|---|
| Data Duplikat | Tidak ada | Integrasi Data | Tidak ada |
| Data Hilang (Missing) | Ada | Data Inkonsisten | Tidak ada |
| Standar Format Data | Tidak ada | Outlier (Pencilan) | Ada |

## Bagian 3: Visualisasi Data
