# NLP-Natural-Language-Processing

Code diatas merupakan implementasi untuk melakukan web scraping data ulasan aplikasi Grab dari Google Play Store, melakukan preprocessing pada data ulasan tersebut, memberikan label sentimen pada setiap ulasan, melakukan analisis TF-IDF untuk representasi teks, serta mengaplikasikan algoritma Naive Bayes untuk klasifikasi sentimen. 

Berikut link PPT: 
https://www.canva.com/design/DAGcLsTA5-g/odQneeK4S6NRtP_6xFFWpg/view?utm_content=DAGcLsTA5-g&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h5e70aadacd

Untuk keterangan lebih jelasnya dapat dilihat pada link berikut: 
https://drive.google.com/file/d/1N-YtII_aGDfXYQNEj0Lp0Et_kPV-fE4T/view?usp=sharing

Berikut adalah interpretasi dari setiap bagian kode:

## Web Scraping:

* Menggunakan package google_play_scraper untuk mengambil ulasan aplikasi Grab dari Google Play Store.
* Menyimpan data ulasan dalam format dataframe dan menyimpannya dalam file Excel.

## Preprocessing:

* Menggunakan library Sastrawi untuk proses stemming (mengubah kata ke bentuk dasarnya) dan penghapusan kata-kata stopword (kata-kata umum yang tidak memberikan informasi signifikan).
* Melakukan pembersihan teks dengan menghilangkan karakter khusus, mengonversi teks menjadi lowercase, dan menghapus kata-kata yang tidak dibutuhkan.
* Hasil pembersihan disimpan dalam file Excel.

## Labeling Sentimen:

* Menggunakan kamus sentimen dari file 'NRC.xlsx' untuk memberikan label positif, negatif, atau netral pada setiap ulasan.
* Menyimpan data ulasan yang sudah diberi label sentimen dalam file Excel.

## Data Exploration:

* Menampilkan distribusi sentimen ulasan dengan diagram pie.

## TF-IDF Analysis:

* Menggunakan TfidfVectorizer dari scikit-learn untuk menghitung TF-IDF pada data ulasan.
* Menampilkan jumlah fitur dan matriks TF-IDF.

## Sentiment Analysis using Naive Bayes:

* Membagi dataset menjadi data training dan data testing.
* Menggunakan algoritma Naive Bayes untuk melakukan klasifikasi sentimen.
* Menampilkan tabel confusion matrix, accuracy, precision, recall, dan F1-score.
