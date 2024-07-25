# Waralaba-Model-Fitness - Pengembangan-Bisnis-Strategi-Retensi-Pelanggan
# Pendahuluan <a id='intro'></a>

Permasalahan utama yang dihadapi adalah fenomena pelanggan berhenti atau customer churn, yang seringkali menjadi masalah penting dalam bidang layanan kebugaran. Kesadaran kami terhadap kesulitan melacak dan memahami dengan tepat kapan seorang pelanggan benar-benar berhenti menggunakan produk atau layanan kami telah meningkat. Itulah sebabnya, kami merasa perlu untuk mengembangkan rencana strategis dengan menggunakan pendekatan analitik berbasis data guna mengatasi masalah ini. 

Dalam hal ini, perhatian utama dari proyek ini adalah untuk mengevaluasi data pelanggan yang telah kami ubah menjadi bentuk digital. Kami meyakini bahwa dengan memiliki pemahaman yang lebih mendalam mengenai perilaku dan preferensi pelanggan, kami dapat mendeteksi kemungkinan pelanggan berhenti menggunakan layanan sebelum hal itu benar-benar terjadi. Dengan pendekatan ini, kami dapat mengembangkan strategi retensi pelanggan yang lebih efisien, menyesuaikan layanan kami sesuai dengan kebutuhan masing-masing individu, dan memperkuat hubungan kami dengan setiap anggota komunitas fitness yang kami miliki. 

Melalui proyek ini, kami ingin mengurangi angka pindah pelanggan, meningkatkan kesetiaan konsumen, dan akibatnya, meningkatkan kelangsungan bisnis kami. Dengan komitmen untuk menyediakan pengalaman fitness yang tak terlupakan, kami percaya bahwa strategi berorientasi data ini akan membawa Model Fitness mencapai kesuksesan yang lebih tinggi. Kami mengucapkan terima kasih atas partisipasi dan kerja sama Anda dalam melaksanakan proyek ini bersama tim kami. Ayo kita bersama-sama mencapai keberhasilan! 

# Tujuan <a id='GoalSet'></a>

Maksud dan tujuan dari project yang akan kami bahas diantaranya:

1. Mempelajari cara memprediksi probabilitas churn (untuk bulan berikutnya) bagi setiap pelanggan
2. Membuat segmentasi pengguna dengan memilih kelompok yang paling dominan dan mendeskripsikan fitur-fitur utamanya
3. Menganalisis faktor yang paling memengaruhi churn
4. Menarik kesimpulan dasar dan memberikan rekomendasi terkait cara meningkatkan layanan pelanggan
5. Mengidentifikasi kelompok yang ditargetkan
6. Merekomendasikan langkah-langkah untuk mengurangi churn
7. Mendeskripsikan pola lain yang kamu temui terkait interaksi pelanggan

# Tahapan yang dilakukan<a id='StepbyStep'></a>

Tahapan-tahapan yang akan dilakukan adalah sebagai berikut:

**1. Memuat file data dan pelajari informasi umumnya. File path: /datasets/gym_churn_us.csv**

**2. Melakukan analisis data eksploratif (EDA):**

Perhatikan dataset yang tersedia, apa ada fitur yang hilang?󠀲󠀡󠀥󠀥󠀧󠀨󠀣󠀠󠀳󠀰 Pelajari nilai rata-rata dan standar deviasinya (gunakan metode describe()).󠀲󠀡󠀥󠀥󠀧󠀨󠀣󠀡󠀳
Lihat nilai fitur rata-ratanya dalam dua kelompok, yaitu untuk mereka yang keluar (churn) dan untuk mereka yang tinggal (gunakan metode groupby()).󠀲󠀡󠀥󠀥󠀧󠀨󠀣󠀢󠀳
Buat histogram dan distribusi fitur untuk mereka yang keluar (churn) serta mereka yang tinggal.󠀲󠀡󠀥󠀥󠀧󠀨󠀣󠀣󠀳
Buat matriks korelasi dan tampilkan hasilnya.

**3. Membangun model untuk memprediksi churn pengguna:**

Bagi datanya menjadi train set dan validation set menggunakan fungsi train_test_split().󠀲󠀡󠀥󠀥󠀧󠀨󠀣󠀨󠀳
Latih model pada train set dengan dua metode berikut:
regresi logistik
random forest
Evaluasi accuracy, precision, dan recall untuk kedua model menggunakan validation set.󠀲󠀡󠀥󠀥󠀧󠀨󠀤󠀢󠀳󠀰 Gunakan metrik-metrik tersebut untuk membandingkan model.󠀲󠀡󠀥󠀥󠀧󠀨󠀤󠀣󠀳󠀰 Model mana yang memberikan hasil terbaik?

**4. Membuat klaster pengguna:**

Lakukan standardisasi terhadap data.󠀲󠀡󠀥󠀥󠀧󠀨󠀤󠀩󠀳
Gunakan fungsi linkage() untuk membuat matriks jarak berdasarkan matriks fitur yang telah distandardisasi dan buat grafik dendrogram.󠀲󠀡󠀥󠀥󠀧󠀨󠀥󠀠󠀳󠀰 Catatan: sabar ya, pembuatan dendrogram mungkin butuh waktu lebih!󠀲󠀡󠀥󠀥󠀧󠀨󠀥󠀡󠀳󠀰 Gunakan grafik yang dihasilkan untuk memperkirakan jumlah klaster yang bisa kamu pilih.󠀲󠀡󠀥󠀥󠀧󠀨󠀥󠀢󠀳
Latih model pengklasteran dengan algoritma K-means dan prediksikan klaster pelanggannya. (Tetapkan jumlah klasternya menjadi n=5 sehingga akan lebih mudah untuk membandingkan hasil yang kamu dapat dengan hasil dari siswa lain.󠀲󠀡󠀥󠀥󠀧󠀨󠀥󠀣󠀳󠀰 Namun ingat ya, di kehidupan nyata tidak akan ada yang memberimu petunjuk seperti itu. Oleh karena itu ke depannya, kamu harus membuat keputusan berdasarkan grafik dari langkah sebelumnya.)󠀲󠀡󠀥󠀥󠀧󠀨󠀥󠀤󠀳
Lihat nilai rata-rata fitur untuk semua klaster.󠀲󠀡󠀥󠀥󠀧󠀨󠀥󠀥󠀳󠀰 Apa ada yang menarik perhatianmu?󠀲󠀡󠀥󠀥󠀧󠀨󠀥󠀦󠀳
Buat grafik distribusi fitur untuk setiap klaster.󠀲󠀡󠀥󠀥󠀧󠀨󠀥󠀧󠀳󠀰 Apa kamu memperhatikan sesuatu?
Hitung tingkat churn untuk setiap klaster (gunakan metode groupby()).󠀲󠀡󠀥󠀥󠀧󠀨󠀥󠀩󠀳󠀰 Apa klaster-klaster tersebut berbeda sehubungan dengan tingkat churn?󠀲󠀡󠀥󠀥󠀧󠀨󠀦󠀠󠀳󠀰 Klaster pelanggan mana yang cenderung akan pergi, dan mana yang akan tetap setia?

**5. Merumuskan kesimpulan dan rekomendasi sederhana untuk bekerja dengan pelanggan.**
