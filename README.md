# Proyek Pertama: Menyelesaikan Permasalahan Human Resources

## Business Understanding
Jaya Jaya Maju merupakan salah satu perusahaan multinasional yang telah berdiri sejak tahun 2000. Ia memiliki lebih dari 1000 karyawan yang tersebar di seluruh penjuru negeri. 

### Permasalahan Bisnis
Walaupun telah menjadi menjadi perusahaan yang cukup besar, Jaya Jaya Maju masih cukup kesulitan dalam mengelola karyawan. Hal ini berimbas tingginya attrition rate (rasio jumlah karyawan yang keluar dengan total karyawan keseluruhan) hingga lebih dari 10%.

### Cakupan Proyek
Menganalisa Berbagai Faktor yang mempengaruhi attrition rate pada perusahaan Jaya Jaya Maju dan membuat dashboard untuk memonitor faktor tersebut.
1. Rentang usia berapa pekerja cenderung melakukan attrition?
2. Apakah terdapat korelasi antara work life balance dengan attrition? Pada rentang nilai berapa pekerja cenderung melakukan attrition?
3. Pekerja dengan tingkat job involvement (keterlibatan dalam pekerjaan) mana yang paling banyak melakukan attrition di perusahaan?
4. Pada rentang waktu berapa lama pekerja cenderung melakukan attrition?
5. Pada rentang nilai berapa Monthly Rate pekerja cenderung meninggalkan perusahaan?
6. Apakah terdapat korelasi antara Monthly Income dengan tingkat attrition?
7. Bagaimana peran jarak tempat tinggal dan kantor dalam keputusan pekerja untuk melakukan attrition?

Analisis faktor-faktor yang mempengaruhi attrition rate pada perusahaan Jaya Jaya Maju dilakukan dengan menggunakan KMeans Clustering. Feature yang digunakan untuk melakukan clustering antara lain:
1. Age
2. WorkLifeBalance
3. YearsAtCompany
4. JobInvolvement
5. MonthlyRate
6. MonthlyIncome
7. DistanceFromHome

Evaluasi pada model yang telah dibuat menggunakan metrik inertia dan silhouette coefficient.

### Persiapan
Sumber data: https://raw.githubusercontent.com/dicodingacademy/dicoding_dataset/main/employee/employee_data.csv

Setup Environment 

import pandas as pd



## Business Dashboard
<div align="center">
  
![image](https://github.com/astriwidyastiti/human_resources_analysis/assets/81604461/c3675c91-7ba8-4b2a-ac2a-ae4d96c05724)

</div>

Untuk mengakses dashboard tersebut dapat melalui link https://lookerstudio.google.com/reporting/f181caa2-827d-4c48-a92c-4ac7defbe61a

Pada perusahaan Jaya Jaya Maju terdapat total 1470 total karyawan yang terdaftar, 179 sudah berpindah perusahaan.

Adapun beberpa faktor yang dapat dilihat dari dashboard tersebut dan harapannya dapat membantu HR dalam memantau faktor tersebut, diantaranya :

1. Gender = Dalam dashboard dapat terlihat bahwa karyawan yang berpindah perusahaan sebesar 60,3 % adalah laki-laki
2. Job Role = Dalam dashboard dapat dilihat bahwa pekerja yang melakukan attrition paling banyak adalah Laboratory Technician
3. Departments = Dalam dashboard dapat dilihat bahwa department yang banyak kehilangan pekerja adalah department Research & Developments sebesar 59,8%
4. Work Life Balance = Dalam dashboard dapat terlihat bahwa karyawan yang berpindah perusahaan terbesar memiliki work life balance rating 3, dimana jika dikategorikan score rating 3 tidak terlalu buruk.
5. Age = Dalam dashboard dapat terlihat bahwa karyawan yang berpindah perusahaan terbanyak pada umur 31
6. Years At Company = Dalam dashboard dapat terlihat bahwa karyawan yang paling banyak melakukan attrition adalah pekerja yang bekerja pada tahun pertama.
7. Distance From Home = Dalam dashboar terlihat bahwa pekerja yang melakukan attrition adalah pekerja yang tinggal tidak jauh dari perushaan.

## Conclusion
Berdasarkan hasil analisis dengan menggunakan kmeans clustering : Pekerja yang paling banyak melakukan attrition adalah pekerja yang berada pada segment 2

<div align="center">
  
![segment](https://github.com/astriwidyastiti/human_resources_analysis/assets/81604461/36eeaf1b-d17e-43c2-b214-60384e3d5410)

</div>

Visualisasi masin-masing segment:

<div align="center">
  
![visualize](https://github.com/astriwidyastiti/human_resources_analysis/assets/81604461/b13845b5-9eae-44ee-b5ca-ea207a5d4a97)

</div>

Berdasarkan hasil clustering dengan menggunakan kMeans dan visualisasi masing-masing faktor, didapatkan bahwa pekerja yang banyak melakukan attrition adalah pekerja dengan karakteristik berikut:
1. Pekerja yang memiliki usia di antara 25 tahun hingga 35 tahun
2. Pekerja yang memiliki nilai worklife balance 3 hingga 4 (excellent-outstanding)
3. Pekerja yang sudah bekerja kurang lebih 1-5 tahun
4. Pekerja yang memiliki job involvement (keterlibatan selama bekerja) dengan nilai 2 hingga 3 (medium-high)
5. Pekerja yang memiliki Monthly Rate di antara 5000 hingga 10000
6. Pekerja yang memiliki Monthly Income lebih dari di antara 2500 hingga 5000
7. Pekerja yang memiliki jarak tempat tinggal dan kantor berada di rentang kurang dari 5km.

### Rekomendasi Action Items
1. Dilihat dari pekerja yang melakukan attrition berada pada rentang usia 25-35 tahun, di mana usia tersebut tergolong muda. Perusahaan sebaiknya menerapkan mentoring pada pekerja di mana pekerja muda dapat belajar dari pekerja yang lebih senior.
2. Perusahaan menawarkan jam kerja yang fleksibel atau opsi bekerja dari rumah untuk membantu pekerja mengelola pekerjaan dan kehidupan pribadi.
3. Perusahaan memberikan penghargaan kepada pekerja yang telah mencapai waktu tertentu dalam perusahaan (misalnya setiap tahun mendapatkan reward).
4. Untuk meningkatkan keterlibatan pekerja perusahaan sebaiknya melibatkan pekerja dalam pengambilan keputusan yang berhubungan dengan pekerjaan mereka.
5. Perusahaan sebaiknya mengimplementasikan skema bonus dan insentif berdasarkan kinerja untuk meningkatkan motivasi pekerja.
6. Perusahaan menciptakan program komunitas atau klub di lingkungan kantor yang dapat meningkatkan rasa kebersamaan di antara pekerja yang memiliki tempat tinggal yang dekat dengan kantor.
