# Process-Data-from-Dirty-to-Clean
Define data integrity, including types and risks, apply SQL functions to clean string variables, develop SQL queries for databases, and describe the process of verifying cleaned data results.
Di sini kita akan mempelajari tentang integritas data, termasuk jenis-jenisnya dan risiko-risikonya. Kemudian, kita akan mempraktikkan penerapan fungsi SQL untuk membersihkan variabel string, merancang kueri SQL untuk bekerja dengan basis data, dan menjelaskan langkah-langkah verifikasi hasil data yang telah dibersihkan.

# Module 1: The Importance of Integrity
" Ketika kita mulai memikirkan cara menyiapkan data untuk eksplorasi, bagian ini dari kursus akan menyoroti mengapa integritas data begitu penting untuk pengambilan keputusan yang berhasil. Kita akan mempelajari bagaimana data dihasilkan dan teknik analis yang digunakan untuk menentukan data mana yang akan dikumpulkan untuk analisis. Selain itu, kita akan mengetahui tentang data terstruktur dan tidak terstruktur, jenis data, dan format data." 

Contoh code yang jelas:
```python
## Contoh code Python untuk membersihkan data dan mengidentifikasi jenis data
import pandas as pd

## Membaca data dari file CSV
data = pd.read_csv('dataset.csv')

## Menampilkan lima baris pertama data
print(data.head())

## Memeriksa jenis data dalam setiap kolom
print(data.dtypes)

## Menghitung jumlah data yang hilang dalam setiap kolom
print(data.isnull().sum())
```

# Module 2: Sparkling-clean Data
Every data analyst wants clean data to work with when performing an analysis. In this part of the course, you’ll learn the difference between clean and dirty data. You’ll also explore data cleaning techniques using spreadsheets and other tools.

```python
import pandas as pd
import pandas as pd
# Contoh DataFrame dengan data yang perlu dibersihkan
data = {'Nama': ['John', 'Jane', 'Bob', 'Alice'],
        'Usia': [25, 'Unknown', 30, 28],
        'Gaji': ['$5000', '$6000', '$4500', '$5500']}

df = pd.DataFrame(data)

# Menampilkan DataFrame sebelum pembersihan
print("DataFrame Sebelum Pembersihan:")
print(df)

# Membersihkan data, mengganti nilai 'Unknown' dengan NaN, dan menghapus simbol dollar dari kolom 'Gaji'
df['Usia'] = pd.to_numeric(df['Usia'], errors='coerce')
df['Gaji'] = df['Gaji'].replace('[\$,]', '', regex=True).astype(float)

# Menampilkan DataFrame setelah pembersihan
print("\nDataFrame Setelah Pembersihan:")
print(df)
```
# Module 3: Cleaning Data with SQL
Knowing a variety of ways to clean data can make an analyst’s job much easier. In this part of the course, you’ll check out how to clean your data using SQL. You’ll explore queries and functions that you can use in SQL to clean and transform your data to get it ready for analysis.

# Module 4: Verify and report on your cleaning results
Cleaning data is an essential step in the data analysis process. Verifying and reporting our cleaning is a way to show that our data is ready for the next step. In this part of the course, we'll find out the processes involved with verifying and reporting data cleaning as well as their benefits.

# Module 5: Adding Data to Our Resume
Creating an effective resume will help you on your data analytics career path. In this part of the course, you’ll learn all about the job application process with a focus on crafting a resume that highlights your strengths and applicable experience. Even if you aren't applying to jobs yet, it's still a good time to improve your resume. It's like spring training for a first season in a major league–you don't want to miss it!

# Modul 6: Course Challange
