# HOUSE-PRICE-PREDICTIONS-IN-CALIFORNIA
![image](https://github.com/arifian09/HOUSE-PRICE-PREDICTIONS-IN-CALIFORNIA/assets/151009269/5d6311ca-66f0-41d5-ba67-ac405de65c40)
Project ini merupakan project capstone dari modul III program Job Connector Data Science di Purwadhika Digital Technology School yang telah mempelajari Machine Learning. project ini bertujuan untuk mengimplementasikan materi yang telah dipelajari tersebut kedalam sebuah project.

Yang ditekankan dalam project ini adalah membuat prediksi harga rumah terbaik dalam data yang sudah dipilih yaitu dataset california housing. Fokus dalam project ini adalah pencarian algoritma terbaik dengan membandingkan beberapa algoritma.

![image](https://github.com/arifian09/HOUSE-PRICE-PREDICTIONS-IN-CALIFORNIA/assets/151009269/d6eb7ca4-c4d8-4428-9d70-6693bbb18ab8)
Pertambahan populasi tentu menyebabkan kebutuhan akan tempat tinggal menjadi penting. Disamping itu, pembangunan rumah bersifat irreversible, maksudnya tidak bisa diulang sehingga harus benar-benar diperhitungkan untuk penetapan harganya. Harga yang terlalu mahal akan membuat properti tidak laku, sedangkan harga terlalu murah membuat margin tidak maksimal jadi kita bisa bilang penetapan harga rumaah yang sesuai adalah kunci.

![image](https://github.com/arifian09/HOUSE-PRICE-PREDICTIONS-IN-CALIFORNIA/assets/151009269/cb7f4e70-0fcc-4fce-84ef-ce6b3e9d6682)
Presentasi ini diperuntukan untuk C-level developer property yang akan membangun rumah dikawasan ini (california). Problem yang akan kita coba solved adalah menentukan harga rumah yang yang tepat dan sesuai. Goals yang akan kita tuju adalah prediksi harga rumah terbaik menggunakan pendekatan computer science. Analytical approach yang akan kita gunakan adalah model regresi, sesuai dengan kecocokan data dan untuk matriks evaluasinya kita menggunakan RMSE & R2

![image](https://github.com/arifian09/HOUSE-PRICE-PREDICTIONS-IN-CALIFORNIA/assets/151009269/17c6f87d-1e4e-43a0-a746-6ea70dca557c)
Adapun dataset yang digunakan seperti gambar diatas, ada 10 kolom dengan target yang adalah median house value sedangkan kolom lain sebagai fitur. Data ini juga terdapat 207 missing value ditotal bedrooms yang diputuskan diisi dengan media value. Untuk outliers, kita memutuskan untuk tidak melakukan drop semua karena cukup banyak, kita memilih outliers yang paling ekstrim saja supaya tidak mengganggu model machine learning. untuk sebaran data dari fiturnya kebanyakan positif skewness.

![image](https://github.com/arifian09/HOUSE-PRICE-PREDICTIONS-IN-CALIFORNIA/assets/151009269/4dfd71a5-b16c-4d6c-ad6b-28886262753d)

Tahap preprocessing terbagi menjadi beberapa tahap, pertama kita ada penambahan 2 fitur yaitu : Ruangan per rumah tangga (rooms_per_household) dan Ruang tidur per Ruangan (bedrooms_per_room). ini tujuannya untuk memperbanyak fitur sehingga prediksinya diharapkan bisa lebih baik, lalu fitur longitude & latitude, kita tidak lakukan apa-apa karena angka-angka disini hanya mengasosiasikan tempat, tidak berpengaruh secara langsung ke harga rumah, fitur ocean proximity kita lakukan label encoding, karena kita berpendapat bahwa ini mempunyai tingkatan, makin dekat dengan laut, maka makin besar angkanya. diluar fitur itu, kita lakukan log transform karena datanya banyak yang positif skewness. log transform efektif untuk memperlandai skewness data.

![image](https://github.com/arifian09/HOUSE-PRICE-PREDICTIONS-IN-CALIFORNIA/assets/151009269/d8879c59-6145-4749-b70b-bc02aa130d81)
Alasan kita memilih RMSE dan R2 sebagai evaluasi metriks adalah karena menurut sumber yang kita dapatkan, keduanya termasuk mudah untuk diinterpretasikan. Model terbaik menurut RMSE adalah yang bernilai paling kecil yaitu Catboost senilai 0.204017. Sedangkan untuk R-square, model terbaik adalah ketika nilai R-squarenya paling besar yang juga sama yaitu Catboost
dengan nilai 0.854283. Sehingga, kita bisa simpulkan model terbaik adalah Catboost

![image](https://github.com/arifian09/HOUSE-PRICE-PREDICTIONS-IN-CALIFORNIA/assets/151009269/f2e4cd04-788a-4073-b9f0-aa6c72c65317)
kita bisa lihat tabel diatas menunjukan prediksi dengan aktual. ada beberapa data yang mendekati ada yang sedikit jauh, tapi kita rasa model sudah cukup baik. dari tabel kita bisa melihat kecenderungan prediksi lebih kecil dari harga actual.

![image](https://github.com/arifian09/HOUSE-PRICE-PREDICTIONS-IN-CALIFORNIA/assets/151009269/375d9e7f-be68-4fc0-96a6-186de6177822)
Kita bisa mengatakan catboost adalah algoritma terbaik menurut evaluasi matriks yang sudah kita tentukan dengan perlakuan-perlakuan seperti yang sudah dijelaskan sebelumnya.

![image](https://github.com/arifian09/HOUSE-PRICE-PREDICTIONS-IN-CALIFORNIA/assets/151009269/e1431339-9b0e-4376-8c80-66b8fcb8bfd8)
Untuk rekomendasi, penjelasannya seperti yang dislide atas. Ini tentu dari sudut pandang data scientist. untuk mendapatkan konklusi yang utuh, kita perlu mendengar saran dari divisi lain lalu kita rembukan formula terbaik

![image](https://github.com/arifian09/HOUSE-PRICE-PREDICTIONS-IN-CALIFORNIA/assets/151009269/a24047c6-b2d7-4c94-b78b-1aa48ec18603)













