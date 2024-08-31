# Tugas Resume Visualisasi Data dan Informasi

Nama            : Happy Syahrul Ramadhan </br>
NIM             : 122450013 </br>
Dosen Pengampu  : Ahmad Luky Ramdani S.Komp., M.Kom
<br/>
<br/>

# <div align="center">Making Data Visualization more Efficient and Effective</div>

## Introduction
Mengubah data abstrak menjadi representasi visual seperti bentuk, dan warna merupakan cara yang efektif untuk menyampaikan informasi kepada individu yang lebih peka atau impresif terhadap visual. Saat ini, organisasi memiliki lebih banyak data daripada sebelumnya, dan semakin banyak yang menggunakan analitik canggih untuk mendukung keputusan strategis dan operasional. Visualisasi data sangat membantu dalam merangkum informasi yang kompleks, membuatnya lebih mudah dipahami, dan mempermudah para data scientist dalam menyampaikan hasil analisis mereka.

## Alur dalam melakukan visualisasi data 

<img src="https://private-user-images.githubusercontent.com/70791897/363409859-84325e00-7190-4805-922d-12cea5a52018.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjUxMDM0OTUsIm5iZiI6MTcyNTEwMzE5NSwicGF0aCI6Ii83MDc5MTg5Ny8zNjM0MDk4NTktODQzMjVlMDAtNzE5MC00ODA1LTkyMmQtMTJjZWE1YTUyMDE4LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA4MzElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwODMxVDExMTk1NVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWFiYzIxMGMwNzQzNGE5YTNhMzc0ZDMxNDdmMmU5MDY4YWYwNjFjMjQxN2EyNzYwYzEyY2UxMDg1OTQ1Y2VkZjUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.yFtpLDv1DT_eRasopjux6eCiIikxLMEhQ7JqtwdH8h8" width="70%">                   
<br/>
<br/>

<ol>
    <li>Impor data adalah mengambil data yang diperlukan dari sumber data yang diinginkan.</li>
    <li>Persiapan data adalah mempersiapkan data sebelum dilakukan visualisasi, misalnya dengan menormalkan nilai, mengoreksi entri yang salah, dan interpolasi nilai yang hilang.</li>
    <li>Manipulasi data adalah memilih data yang akan divisualisasikan (alias pemfilteran) dan mungkin dengan operasi umum lainnya seperti menggabungkan antar data dan pengelompokan.</li>
    <li>Pemetaan adalah memetakan data yang diperoleh dari atas proses ke primitif geometris (misalnya titik dan garis), beserta atributnya (misalnya, warna, posisi, dan ukuran).</li>
    <li>Rendering adalah mengubah data geometri di atas menjadi representasi visual.</li>
</ol>

Berdasarkan alur di atas, kami telah mengidentifikasi tiga arah yang membuat visualisasi data lebih efisien dan efektif relevan bagi peneliti basis data yaiu : 

<ol>
    <li><b>Visualization Specifications</b> Spesifikasi visualisasi menyediakan berbagai cara agar pengguna dapat menentukan apa yang mereka inginkan. Ada banyak sekali penelitian baik dari visualisasi</li>
    <li><b>Efficient Approaches for Data Visualization</b> Untuk melibatkan pengguna secara efektif dalam iteratif pipeline, proses pembuatan visualisasi data harus dilakukan efisien dan terukur, terutama untuk dua komponen, "Manipulasi Data" dan "Pemetaan". Banyak peneliti telah melakukannya mencoba visualisasi dengan program data yang kuat dan matang mesin penghenti seperti menerjemahkan kueri visualisasi ke kueri SQL untuk dievaluasi melalui RDBMS, dan menyesuaikan sistem yang ada untuk visualisasi data tugas seperti HyperDB untuk Tableau.</li>
    <li><b>Data Visualization Recommendation</b> Menyusun visualisasi yang tepat adalah tugas yang sulit, bahkan bagi para ahli, karena melibatkan pemahaman data, narasi yang ingin disampaikan, dan metode visualisasi yang sesuai, yang sering kali merupakan proses trial and error. Oleh karena itu, penting bagi sistem visualisasi untuk secara cerdas membimbing pengguna dengan memberikan rekomendasi.</li>
</ol>


## Spesifikasi visualisasi
Secara umum, bahasa visualisasi data terdiri dari tiga bagian: data, tanda (atau isyarat visual), dan pemetaan.
<ul>
    <li><b>Data</b></li>
    <ul>
        <li><b>Records</b> : the data that need to be visualized.</li>
        <li><b>Transformation</b> : the operations—such as group, bin, filter, and sort—are used to transform the specified data records.</li>
    </ul>
</ul>
<ul>
    <li><b>Tanda (atau isyarat visual)</b></li>
    <ul>
        <li><b>Type</b> : the visual representation for data records, such as bar, line or point.</li>
        <li><b>Size</b> : the width, height of the visualization.</li>
        <li><b>Legend</b> : the legend information.</li>
        <li><b>Miscellaneous</b> : other properties, such as the width and color of a bar.</li>
    </ul>
</ul>
<ul>
    <li><b>Mapping</b> : maps data to corresponding marks.</li>
</ul>

## Kategorisasi visualisasi data
<img src="https://private-user-images.githubusercontent.com/70791897/363409807-6de9cd98-cb56-4eb0-bf06-9c7d7b0f61f0.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjUxMDM0NTcsIm5iZiI6MTcyNTEwMzE1NywicGF0aCI6Ii83MDc5MTg5Ny8zNjM0MDk4MDctNmRlOWNkOTgtY2I1Ni00ZWIwLWJmMDYtOWM3ZDdiMGY2MWYwLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA4MzElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwODMxVDExMTkxN1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWU0NGExYzk0OTA4ZDQ0NGIxNmI2YzlkZWZkZDcxOTY2MzQyMjRmMjk1MWIyMGE4ZTFjNTY1MjBjZjFlNDg4ODQmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.9OUAkd2027GKQ5yA-ge7IMyVdF720GwKUXvfQV3DJ3E" width="70%">                   

Bahasa visualisasi dapat diklasifikasikan berdasarkan tingkat ekspresifitasnya. Bahasa tingkat rendah memungkinkan pengguna untuk memiliki kendali penuh atas setiap elemen visualisasi, memberikan fleksibilitas maksimum namun membutuhkan lebih banyak usaha. Sebaliknya, bahasa tingkat tinggi menyederhanakan proses dengan memberikan default yang masuk akal dan mengurangi tingkat detail yang harus ditentukan oleh pengguna. Ada juga alat berbasis GUI yang lebih ramah pengguna dan memungkinkan spesifikasi visualisasi melalui manipulasi langsung, serta bahasa yang lebih fleksibel yang mendukung spesifikasi visualisasi yang tidak lengkap.

## Pendekatan Efisien untuk Visualisasi Data
<ul>
    <li><b>Visualisasi Data yang Tepat</b> : Visualisasi data yang tepat atau exact data visualization bertujuan untuk menghasilkan visualisasi yang akurat secepat mungkin. Ini dicapai melalui berbagai teknik seperti Query Translation, di mana kueri visualisasi diterjemahkan ke dalam kueri SQL yang dieksekusi di RDBMS, serta penggunaan penyimpanan berbasis kolom yang lebih efisien untuk operasi OLAP.
    </li>
    <li><b>Visualisasi Data Perkiraan</b> : Dalam situasi di mana visualisasi data yang tepat tidak dapat dihasilkan dengan cepat karena ukuran data yang besar atau kompleksitas kueri yang tinggi, teknik visualisasi data perkiraan digunakan. Teknik ini, seperti AQP (Approximate Query Processing), memungkinkan pembuatan visualisasi yang mendekati hasil akhir dengan menggunakan subset data yang representatif. Pendekatan ini mengorbankan sedikit akurasi untuk memberikan hasil yang lebih cepat dan interaktif.
    </li>
    <li><b>Visualisasi Data Progresif</b> : Visualisasi data progresif memberikan hasil secara bertahap dengan menggunakan struktur hierarkis untuk agregasi data. Misalnya, data dapat dibagi menjadi berbagai level berdasarkan ukuran bin, rentang temporal, atau zona spasial, yang memungkinkan pengguna untuk menjelajahi data secara bertahap. 
    </li>
</ul>

## Rekomendasi Visualisasi
<ul>
    <li><b>Rekomendasi Berdasarkan Spesifikasi</b> : Sistem rekomendasi visualisasi berdasarkan spesifikasi dirancang untuk membantu pengguna dalam memilih visualisasi yang sesuai berdasarkan spesifikasi yang mereka berikan. Jika spesifikasi yang diberikan tidak lengkap atau hanya mencakup sebagian elemen visualisasi, sistem akan memberikan rekomendasi yang relevan berdasarkan spesifikasi tersebut. 
    </li>
    <li><b>Rekomendasi Berdasarkan Perilaku</b> : Selain spesifikasi, beberapa sistem rekomendasi juga mempertimbangkan perilaku pengguna, seperti pola eksplorasi visualisasi yang sering digunakan atau preferensi visualisasi yang sering dipilih. Dengan memanfaatkan data historis dan pola penggunaan, sistem dapat memberikan rekomendasi yang lebih personal dan sesuai dengan kebiasaan pengguna. 
    </li>
    <li><b>Rekomendasi Berdasarkan Perilaku</b> : Selain spesifikasi, beberapa sistem rekomendasi juga mempertimbangkan perilaku pengguna, seperti pola eksplorasi visualisasi yang sering digunakan atau preferensi visualisasi yang sering dipilih. Dengan memanfaatkan data historis dan pola penggunaan, sistem dapat memberikan rekomendasi yang lebih personal dan sesuai dengan kebiasaan pengguna. 
    </li>
    <li><b>Rekomendasi Personalisasi</b> : Rekomendasi personalisasi mempertimbangkan preferensi individu pengguna, baik dari segi gaya visualisasi maupun tipe data yang sering digunakan. Dengan memahami preferensi unik setiap pengguna, sistem dapat memberikan saran yang lebih relevan dan efektif, membantu pengguna untuk dengan cepat menemukan visualisasi yang paling sesuai dengan kebutuhan mereka. Pendekatan ini sering melibatkan pembelajaran mesin untuk mengenali pola preferensi dari interaksi sebelumnya, memungkinkan sistem untuk terus memperbaiki rekomendasi seiring waktu.
    </li>
</ul>

##  Other research directions
### Persiapan Data untuk Visualisasi 
<ul>
    <li><b>Kebersihan Data</b> : Data dunia nyata sering kali tidak bersih, yang dapat menyesatkan pengguna saat divisualisasikan.</li>
    <li><b>Analisis What-If untuk Outliers</b> : Sistem seperti Scorpion memungkinkan pengguna untuk mengidentifikasi outlier secara manual dan kemudian menghapus predikat yang menyebabkan outlier tersebut tanpa mempengaruhi data lainnya.</li>
    <li><b>Evaluasi Visualisasi dengan Data yang Hilang</b> : Penelitian juga dilakukan untuk mengevaluasi faktor-faktor yang mempengaruhi akurasi respons, kualitas data, dan kepercayaan dalam interpretasi data deret waktu dengan nilai yang hilang.</li>
</ul>

### Benchmark untuk Visualisasi Data
<ul>
    <li><b>Pentingnya Benchmark</b> : Sama seperti ImageNet atau TPC benchmarks klasik, penting untuk mengembangkan benchmark yang setia pada tugas analisis visual, menyediakan jejak data yang dapat digunakan kembali, dan memiliki cakupan serta kualitas label yang tinggi untuk rekomendasi visualisasi.</li>
    <li><b>Proyek VizNet</b> : VizNet telah menyajikan korpus besar lebih dari 31 juta dataset yang dikompilasi dari repositori data terbuka dan galeri visualisasi online.</li>
</ul>

### Visualisasi Data untuk Aplikasi Terkait Basis Data
<ul>
    <li><b>Data visualization for data discovery</b> : Penemuan data, yaitu menemukan dataset yang menarik untuk aplikasi tertentu dari data lake yang berisi ribuan atau jutaan data, masih merupakan masalah yang sulit untuk dipecahkan.</li>
    <li><b>Visualisasi Data untuk Debugging Data</b> : Masalah lain yang baru-baru ini diangkat oleh sistem Data Civilizer adalah debugging data, di mana output dari workflow analitik data salah bukan karena bug dalam program, tetapi karena data yang salah seperti input yang salah atau parameter yang salah.</li>
</ul>

