# Proyek Akhir : Menyelesaikan Permasalahan Perusahaan Jaya Jaya Maju

## Business Understanding
Perusahaan Jaya Jaya Maju menghadapi masalah tingginya tingkat keluarnya karyawan (attrition). Walaupun telah menjadi menjadi perusahaan yang cukup besar, Jaya Jaya Maju masih cukup kesulitan dalam mengelola karyawan. Hal ini berimbas tingginya attrition rate (rasio jumlah karyawan yang keluar dengan total karyawan keseluruhan) hingga lebih dari 10%. Oleh karena itu, perlu dianalisis faktor-faktor yang mempengaruhi tingkat keluarnya karyawan untuk membantu departemen HR dalam mengurangi tingkat attrition.

## Dataset ini terdiri dari 34 feature atau kolom :
- EmployeeId - Employee Identifier
- Attrition - Did the employee attrition? (0=no, 1=yes)
- Age - Age of the employee
- BusinessTravel - Travel commitments for the job
- DailyRate - Daily salary
- Department - Employee Department
- DistanceFromHome - Distance from work to home (in km)
- Education - 1-Below College, 2-College, 3-Bachelor, 4-Master,5-Doctor
- EducationField - Field of Education
- EnvironmentSatisfaction - 1-Low, 2-Medium, 3-High, 4-Very High
- Gender - Employee's gender
- HourlyRate - Hourly salary
- JobInvolvement - 1-Low, 2-Medium, 3-High, 4-Very High
- JobLevel - Level of job (1 to 5)
- JobRole - Job Roles
- JobSatisfaction - 1-Low, 2-Medium, 3-High, 4-Very High
- MaritalStatus - Marital Status
- MonthlyIncome - Monthly salary
- MonthlyRate - Mounthly rate
- NumCompaniesWorked - Number of companies worked at
- Over18 - Over 18 years of age?
- OverTime - Overtime?
- PercentSalaryHike - The percentage increase in salary last year
- PerformanceRating - 1-Low, 2-Good, 3-Excellent, 4-Outstanding
- RelationshipSatisfaction - 1-Low, 2-Medium, 3-High, 4-Very High
- StandardHours - Standard Hours
- StockOptionLevel - Stock Option Level
- TotalWorkingYears - Total years worked
- TrainingTimesLastYear - Number of training attended last year
- WorkLifeBalance - 1-Low, 2-Good, 3-Excellent, 4-Outstanding
- YearsAtCompany - Years at Company
- YearsInCurrentRole - Years in the current role
- YearsSinceLastPromotion - Years since the last promotion
- YearsWithCurrManager - Years with the current manager

## Permasalahan Bisnis
Tingkat keluarnya karyawan yang tinggi di perusahaan Jaya Jaya Maju menyebabkan berbagai masalah bisnis yang signifikan. Berikut adalah beberapa permasalahan bisnis utama yang dihadapi oleh perusahaan:

1. Produktivitas Menurun Kehilangan karyawan dapat mengakibatkan penurunan produktivitas tim dan keseluruhan perusahaan. Pengalaman dan pengetahuan yang dimiliki karyawan lama sulit untuk digantikan dalam waktu singkat.
2. Gangguan dalam Operasional Kehilangan karyawan secara tiba-tiba dapat mengganggu alur kerja dan menyebabkan proyek atau tugas tertunda. Ini dapat berdampak negatif pada kualitas layanan yang diberikan kepada klien.
3. Kepuasan Karyawan Menurun Tingginya tingkat keluarnya karyawan dapat mempengaruhi moral dan kepuasan karyawan yang masih bertahan.
4. Reputasi Perusahaan Terancam Jika tingkat keluarnya karyawan terus tinggi, reputasi perusahaan sebagai tempat kerja yang stabil dan mendukung bisa terancam. Ini dapat mempengaruhi perusahaan untuk mencari pekerja dimasa depan

## Cakupan Proyek
1. Mengumpulkan dan memproses data karyawan.
2. Menganalisis data untuk menemukan pola dan faktor-faktor yang mempengaruhi keluarnya karyawan.
3. Membangun model prediktif menggunakan algoritma Logistic Regression.
Membuat dashboard bisnis untuk memvisualisasikan temuan dan prediksi.
Memberikan rekomendasi tindakan berdasarkan hasil analisis.

## persiapan
Berikut adalah tahapannya :
sumber data: https://github.com/dicodingacademy/dicoding_dataset/tree/main/employee

## SetUp Environtment
Apabila menginstal Python melalui Anaconda ataupun miniconda, Anda dapat menggunakan conda sebagai package manager dan environment management system. Berikut merupakan tahapan dalam membuat virtual environment menggunakan conda untuk melakukan prediksi.

1. Buka terminal atau PowerShell.
2. Jalankan perintah berikut.
    ```
     conda create --name prediksi_attrition python=3.9
    ```
3. Aktifkan virtual environment dengan menjalankan perintah berikut.
    ```
    conda activate prediksi_attrition
    ```
4. Instal semua library yang dibutuhkan menggunakan perintah berikut.
    ```
    pip install numpy==1.24.4 pandas==2.1.4 matplotlib==3.7.5 seaborn==0.13.2 scikit-learn==1.4.0 SQLAlchemy==2.0.30
    ```
5. Buka jupyter-notebook dengan menjalankan perintah berikut.
    ```
    jupyter-notebook
    ```
6. Buka file python prediction.py
7. Masukkan data yang ingin diprediksi pada variabel X_new
8. Tekan tombol run code
8. Hasil prediksi akan keluar

## Business Dashboard
Dashboard bisnis dibuat untuk memvisualisasikan data karyawan, tingkat keluarnya karyawan, dan faktor-faktor yang mempengaruhi tingginya attrition rate. Dashboard ini akan menampilkan faktor demografi dan penghasilan karyawan, faktor kepuasan dan pekerjaan, faktor keseimbangan kerja dan kehidupan yang mempengaruhi tingginya attrition rate.

## Conclusion
Karyawan yang keluar cenderung berusia muda dan belum menikah, memiliki gaji pokok yang relatif kecil namun mendapatkan penghasilan tambahan yang lebih besar. Mereka sering kesulitan menyeimbangkan pekerjaan dengan kehidupan pribadi, merasa tidak nyaman dengan lingkungan kerja, terutama dalam hubungan dengan atasan. Selain itu, karyawan yang jarang mendapatkan promosi juga lebih rentan untuk keluar. Tingkat attrition yang tinggi terlihat pada bidang pekerjaan seperti teknisi laboratorium, sumber daya manusia, dan peneliti. Karyawan dengan latar belakang pendidikan di bidang teknik dan pemasaran juga menunjukkan kecenderungan keluar yang lebih besar.

## Rekomendasi Action Items
Berikut adalah 4 poin rekomendasi utama yang dapat dilakukan perusahaan Jaya Jaya Maju untuk mengurangi tingkat attrition:

1. BusinessTravel dan Work-Life Balance
Evaluasi kebutuhan perjalanan dinas secara rutin dan cari alternatif seperti rapat virtual. Pertimbangkan kebijakan untuk mengurangi jam kerja tambahan (overtime) dan dorong keseimbangan kehidupan kerja yang lebih baik.

2. Department dan Job Role
Lakukan analisis mendalam terhadap departemen dengan tingkat attrition tinggi seperti R&D dan Sales, serta peran seperti Laboratory Technician dan Sales Executive. Tinjau ulang beban kerja, peluang pengembangan karir, dan kompensasi untuk meningkatkan kepuasan kerja.

3. Environment Satisfaction dan Performance Rating
Tingkatkan kepuasan lingkungan kerja melalui program kesejahteraan dan komunikasi internal yang lebih baik. Pastikan karyawan menerima feedback yang jelas dan dukungan pengembangan karir untuk meningkatkan kepuasan dan kinerja mereka.

4. Compensation, Benefits, dan Training
Tinjau kembali struktur kompensasi untuk memastikan keadilan dan daya saing di industri. Tingkatkan investasi dalam pelatihan dan pengembangan karir agar setiap karyawan memiliki akses yang setara terhadap peluang pertumbuhan.

