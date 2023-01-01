# Classification-Model-for-Loan-Default-Risk-Prediction-Virtual-Internship-Program-Home-Credit

# Problem Statement

Masalah bisnis yang sedang dihadapi adalah terkait pinjaman yang diberikan kepada customer, sebagian diantaranya mengalami keterlambatan/ kesulitan pembayaran. 

![image](https://user-images.githubusercontent.com/114457985/210165533-6a33cfd6-cdb0-4f82-8cff-2c77126faa59.png)



Goals : 
- Menurunkan difficulty payment rate of customer

Objective : 
- Memprediksi customer yang lancar dalam pembayaran
- Menemukan faktor penting dari customer yang lancar dalam pembayaran

Dataset : 
- application_{train|test}
- Bureau


# Top Insight & Recommendation

- Accountant dan High Skill Tech Staff adalah 2 tipe pekerjaan dimana proporsi keberhasilan pembayaran paling tinggi, di atas rata-rata smoothness rate secara keseluruhan. Sedangkan Low-skill Laborers memiliki proporsi kelancaran pembayaran terendah dibandingkan tipe pekerjaan lain.
- Semakin banyak kontrak aktif yang dimiliki customer, kecenderungan pembayarannya semakin sulit.

Recommendation :
- Proporsi tipe Accountant dan High Skill Tech Staff masih di bawah 5%. Oleh karena itu, perusahaan dapat mengoptimalkan kegiatan marketing untuk konsumen yang potensial pada tipe tersebut agar tertarik mengajukan pinjaman. 
- Perusahaan harus berhati-hati pada customer yang memiliki banyak kontrak aktif terutama jumlah kontrak aktif di atas 5


# Modeling 

- Metric yang akan digunakan pada model ini adalah Recall dengan tujuan mengurangi False Negative sebanyak mungkin. False Negative pada case ini adalah debitur yang diprediksi 'LANCAR BAYAR' namun ternyata pada kenyataannya 'KESULITAN BAYAR', kami ingin menghindari hal tersebut yang terjadi akibat salah prediksi. 
- Model akhir yang dipilih adalah Light Gradient Boosting Machine dengan menggunakan class weight karena data yang tidak seimbang, dan threshold default 
- Recall yang didapatkan adalah 66% dan AUC 74.04%


# Prediksi pada Data Test Application Test

- Memprediksi customer apakah nantinya lancar atau mengalami kesulitan dan bayar, dan berapa peluang customer lancar bayar.





