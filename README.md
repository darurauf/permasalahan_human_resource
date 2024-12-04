## Business Understanding

Perusahaan ini mengelola data karyawan untuk menganalisis faktor-faktor yang mempengaruhi kinerja, kepuasan kerja, dan retensi karyawan. Dengan pemahaman yang lebih baik tentang karakteristik dan kebutuhan karyawan, perusahaan berupaya meningkatkan produktivitas, mengurangi angka turnover, serta menciptakan lingkungan kerja yang mendukung.

### Permasalahan Bisnis

Perusahaan saat ini menghadapi beberapa permasalahan serius yang dapat mempengaruhi kinerja dan keberlanjutan organisasi. Beberapa permasalahan utama yang perlu diperhatikan adalah:

1. Tingkat Turnover Karyawan yang Tinggi: Banyak perusahaan mengalami tingkat turnover atau attrition karyawan yang tinggi, yang dapat mengakibatkan kerugian signifikan dalam hal biaya rekrutmen dan pelatihan. Hal ini juga berdampak pada moral karyawan yang tersisa dan produktivitas tim secara keseluruhan. Jika tidak segera diatasi, perusahaan berisiko kehilangan talenta berharga, yang dapat memperlambat pertumbuhan dan inovasi.
2. Keseimbangan Kehidupan Kerja yang Buruk: Karyawan sering mengalami tekanan yang berlebihan dan ketidakmampuan untuk mencapai keseimbangan antara pekerjaan dan kehidupan pribadi. Hal ini dapat mengarah pada penurunan produktivitas, peningkatan stres, dan bahkan masalah kesehatan mental di kalangan karyawan. Tanpa langkah-langkah untuk meningkatkan keseimbangan kehidupan kerja, perusahaan dapat menghadapi peningkatan ketidakhadiran dan penurunan kinerja.
3. Ketidakpuasan Kerja yang Meningkat: Terdapat hubungan yang kuat antara pengalaman kerja, perjalanan bisnis, dan kepuasan kerja karyawan. Ketika karyawan merasa tidak puas dengan pengalaman mereka, termasuk perjalanan bisnis yang berlebihan atau tidak sesuai dengan harapan, hal ini dapat menyebabkan rendahnya motivasi dan kinerja. Jika masalah ini berlanjut, perusahaan akan menghadapi risiko kehilangan karyawan berpengalaman yang dapat berkontribusi pada tujuan jangka panjang organisasi.

Urgensi dan Dampak Jangka Panjang:

Urgensi untuk mengatasi masalah-masalah ini sangat tinggi. Jika perusahaan tidak melakukan tindakan korektif, dampak jangka panjangnya bisa sangat merugikan, termasuk reputasi perusahaan yang buruk di pasar tenaga kerja, kesulitan dalam menarik dan mempertahankan talenta, serta penurunan dalam efisiensi operasional. Oleh karena itu, penting untuk melakukan analisis yang mendalam dan merancang strategi yang efektif untuk mengatasi permasalahan ini demi mencapai keberlanjutan dan pertumbuhan perusahaan di masa depan.

### Cakupan Proyek

Proyek ini bertujuan untuk melakukan analisis mendalam terhadap data demografi, pekerjaan, dan kepuasan karyawan guna memahami faktor-faktor yang berkontribusi terhadap tingkat attrition karyawan. Berikut adalah rincian cakupan proyek:

1. Pekerjaan yang Akan Dilakukan:
Pengumpulan Data: Mengumpulkan data terkait demografi karyawan (usia, pendidikan, dll) dan data pekerjaan (jabatan, lama bekerja, gaji)
2. Praproses Data: Melakukan pembersihan data untuk menghilangkan missing values, dan melakukan encoding untuk data kategorikal. Hal ini penting untuk memastikan data yang digunakan dalam analisis akurat dan relevan.
3. Analisis Hubungan Antarvariabel: Menerapkan teknik analisis, seperti analisis korelasi untuk mengeksplorasi hubungan antara variabel-variabel yang berbeda terhadap tingkat attrition.
4. Modeling dan Prediksi: Mengembangkan model prediksi untuk mengidentifikasi faktor-faktor risiko yang berkontribusi terhadap attrition menggunakan teknik machine learning. Model ini diharapkan dapat memberikan wawasan mengenai potensi karyawan yang berisiko tinggi untuk keluar.
5. Visualisasi Data: Membuat dashboard visualisasi yang interaktif untuk mempresentasikan temuan analisis, memudahkan manajemen dalam memahami data, serta memfasilitasi pengambilan keputusan yang berbasis data.

Batasan Proyek:
1. Proyek ini akan fokus pada data karyawan yang tersedia dalam periode tertentu dan tidak mencakup data dari luar sumber yang ditentukan.
2. Analisis akan terbatas pada faktor-faktor yang dapat diukur secara kuantitatif dan kualitatif dari survei yang telah dilakukan.
3. Proyek tidak akan mencakup implementasi dari rekomendasi kebijakan yang dihasilkan.

Target Proyek:
1. Menciptakan pemahaman yang lebih baik mengenai faktor-faktor yang mempengaruhi attrition karyawan.
2. Menghasilkan rekomendasi berbasis data untuk meningkatkan retensi karyawan dan kesejahteraan di tempat kerja.

Output Akhir dari Proyek:
1. Model Prediksi: Sebuah model yang dapat memprediksi karyawan yang berisiko tinggi untuk melakukan attrition.
2. Dashboard Visualisasi Data: Sebuah dashboard interaktif yang menyajikan hasil analisis dan memungkinkan manajemen untuk mengeksplorasi data dengan lebih mendalam.

### Persiapan

Sumber Data yang digunakan adalah employee_data.csv, yang mencakup beberapa kolom penting seperti:

1. EmployeeId: Identifikasi unik untuk setiap karyawan
2. Age: Usia karyawan
3. Attrition: Indikator apakah karyawan telah meninggalkan perusahaan
4. BusinessTravel: Frekuensi perjalanan bisnis
5. Department: Departemen tempat karyawan bekerja
6. WorkLifeBalance: Skala keseimbangan kehidupan kerja
7. YearsAtCompany: Jumlah tahun karyawan bekerja di perusahaan

Setup environment:

```
cd C:\Users\<user>\Downloads
java -jar metabase.jar
http://localhost:3000
```

## Business Dashboard

Dashboard bisnis dapat dibuat untuk memvisualisasikan data-data kunci seperti:

1. Grafik Attrition by Department
Departemen R&D memiliki tingkat attritio tertinggi: Ini mengindikasikan adanya masalah yang cukup serius di departemen R&D, mungkin terkait dengan beban kerja, kepuasan kerja, atau peluang pengembangan karir.
Departemen Sales memiliki tingkat attritio yang cukup tinggi juga: Hal ini bisa jadi karena tekanan kerja yang tinggi di departemen sales, target yang sulit dicapai, atau kompensasi yang kurang kompetitif.

2. Grafik Attrition by Age
Tingkat attritio tertinggi berada di rentang usia 30-37.5 tahun: Kelompok usia ini mungkin sedang berada di tahap karir yang krusial, di mana mereka mencari tantangan dan perkembangan lebih lanjut. Jika perusahaan tidak mampu memberikan hal tersebut, maka mereka cenderung mencari pekerjaan lain.

3. Grafik Attrition by YearsAtCompany
Tingkat attritio cenderung menurun seiring bertambahnya tahun bekerja: Ini menunjukkan bahwa karyawan yang sudah lama bekerja cenderung lebih loyal dan memiliki ikatan yang lebih kuat dengan perusahaan. Namun, lonjakan kecil pada tahun ke-10 dan ke-20 mengindikasikan adanya potensi masalah pada tahun-tahun tersebut.

4. Grafik Attrition by EducationField
Karyawan dengan latar belakang pendidikan Life Sciences memiliki tingkat attritio tertinggi: Ini bisa jadi karena terbatasnya peluang pengembangan karir untuk bidang tersebut di perusahaan, atau adanya tawaran yang lebih menarik dari perusahaan lain.
Karyawan dengan latar belakang pendidikan Medical dan Marketing juga memiliki tingkat attritio yang cukup tinggi: Hal ini menunjukkan bahwa perusahaan perlu memperhatikan kebutuhan spesifik karyawan dari bidang-bidang tersebut.

## Conclusion

Berdasarkan analisis data karyawan, beberapa faktor utama yang mempengaruhi tingkat keluar masuk karyawan (attrition) telah diidentifikasi. Faktor-faktor ini meliputi kepuasan kerja, jarak tempat tinggal ke kantor, pendapatan bulanan, dan keterlibatan dalam pekerjaan. Selain itu, data menunjukkan perbedaan yang signifikan dalam tingkat keluar masuk karyawan di berbagai peran pekerjaan dan departemen, yang bisa menandakan adanya tantangan dalam budaya kerja di beberapa bagian organisasi.

Karakteristik umum dari karyawan yang mengalami attrition meliputi:

1. Jarak Tempuh yang Jauh: Karyawan yang tinggal jauh dari tempat kerja mengalami tekanan tambahan dari waktu perjalanan yang lama, yang dapat berkontribusi pada keputusan untuk mencari pekerjaan yang lebih dekat dengan rumah.
2. Pendapatan yang Tidak Memadai: Karyawan yang merasa bahwa kompensasi yang mereka terima tidak sebanding dengan beban kerja atau kontribusi mereka kepada perusahaan mungkin lebih cenderung untuk meninggalkan pekerjaan mereka.


Dengan memahami faktor-faktor ini dan karakteristik karyawan yang berisiko tinggi untuk keluar, perusahaan dapat merancang strategi yang lebih efektif untuk meningkatkan retensi karyawan dan menciptakan lingkungan kerja yang lebih mendukung. Upaya ini tidak hanya akan mengurangi tingkat attrition, tetapi juga meningkatkan kepuasan dan keterlibatan karyawan secara keseluruhan, yang pada gilirannya akan berdampak positif pada kinerja organisasi.
