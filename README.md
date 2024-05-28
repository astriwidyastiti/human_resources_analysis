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

### Persiapan
Sumber data: https://raw.githubusercontent.com/dicodingacademy/dicoding_dataset/main/employee/employee_data.csv


## Business Dashboard
![image](https://private-user-images.githubusercontent.com/112534966/334491345-93b411d9-e09b-49f2-a323-d327aaed01e7.jpg?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTY5MTMwNjgsIm5iZiI6MTcxNjkxMjc2OCwicGF0aCI6Ii8xMTI1MzQ5NjYvMzM0NDkxMzQ1LTkzYjQxMWQ5LWUwOWItNDlmMi1hMzIzLWQzMjdhYWVkMDFlNy5qcGc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNTI4JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDUyOFQxNjEyNDhaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT02ODU3MjhmODhhNzZhOTE1NzI5YTJiOGVlMGZjOTFjNjQwNzcxNTU3OTBlYzIyYTY1MjcxM2Q3MjQ3YmNlZjgyJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.ALgAsU5J1SmarRTeKfMZCiRJQgPQQ3EFsVF1UtTHuNw)

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
![image](https://private-user-images.githubusercontent.com/112534966/334496942-ec31dd83-bd71-4278-89e8-bf7d7998ceac.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTY5MTQxMTMsIm5iZiI6MTcxNjkxMzgxMywicGF0aCI6Ii8xMTI1MzQ5NjYvMzM0NDk2OTQyLWVjMzFkZDgzLWJkNzEtNDI3OC04OWU4LWJmN2Q3OTk4Y2VhYy5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNTI4JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDUyOFQxNjMwMTNaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1jMmY3MTYxZWY5ZjQ1NjY0MWMxMWEzZGU3MzVmNmJhMTNlNjkzZDdmZDU5NzdmMmYwZWI4ZmQ3M2QyNWJiYTA3JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.3Yq7hvHbxGhduQ1JtaOvcnxHAiEfm84uGHtqfgeEEMU)

Visualisasi masin-masing segment:

![image](https://private-user-images.githubusercontent.com/112534966/334498400-212a5638-f978-47b0-8cc9-224752a77380.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTY5MTQzNzMsIm5iZiI6MTcxNjkxNDA3MywicGF0aCI6Ii8xMTI1MzQ5NjYvMzM0NDk4NDAwLTIxMmE1NjM4LWY5NzgtNDdiMC04Y2M5LTIyNDc1MmE3NzM4MC5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNTI4JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDUyOFQxNjM0MzNaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0yYTcwZDRmYzg2M2YwOWQxNjdkYTM2MGU2ZDY3ZmNkYjNhZDgyMmMxNzAyZmVmNjE2NTE4ZDJkYjY1NDEyMmQ5JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.8FO4rHxUbCCYvCFU3VeldLdFcg9MIOmgQfyMiNTq1gk)

Berdasarkan hasil clustering dengan menggunakan kMeans dan visualisasi masing-masing faktor, didapatkan bahwa pekerja yang banyak melakukan attrition adalah pekerja dengan karakteristik berikut:
1. Pekerja yang memiliki usia di antara 25 tahun hingga 35 tahun
2. Pekerja yang memiliki nilai worklife balance 3 hingga 4 (excellent-outstanding)
3. Pekerja yang sudah bekerja kurang lebih 1-5 tahun
4. Pekerja yang memiliki job involvement (keterlibatan selama bekerja) dengan nilai 2 hingga 3 (medium-high)
5. Pekerja yang memiliki Monthly Rate di antara 5000 hingga 10000
6. Pekerja yang memiliki Monthly Income lebih dari di antara 2500 hingga 5000
7. Pekerja yang memiliki jarak tempat tinggal dan kantor berada di rentang kurang dari 5km.
