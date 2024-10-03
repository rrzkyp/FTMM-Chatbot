Data dibagi menjadi data training dan testing menggunakan variabel X dan y, dengan masing masing berisi ‘pattern’ dan ‘labels’ yang kemudian menggunakan train_test_split dari sklearn untuk menyeleksi model dengan cara merandom dari size default menggunakan 75% untuk training dan 25% untuk testing.

Pembuatan model BERT beserta tokenizer untuk mengubah teks menjadi bentuk token agar dapat diinputkan ke dalam model BERT dengan menggunakan model yang sudah pernah dibuat sebelumnya.

Data train dan test diubah menjadi bentuk encoding karena sebagian besar model seperti model BERT memerlukan input dalam bentuk representasi angka. 

Definisikan detail spesifikasi variabel untuk training, dengan menggunakan 100 epoch dengan masing-masing 50 step.

Hasil Training mendapatkan Akurasi 1.0 dengan tingkat lost 0.2

Setelah model selesai dilakukan training, hasil model disimpan agar dapat digunakan oleh pengguna lain yang juga ingin membuat chatbot dengan teknik Deep Learning berbasis Semantic Analysis.

Kemudian dilakukan uji coba dengan pertanyaan “TRKB itu bidang mana ya?” dan hasil outputnya memprediksi bahwa pertanyaan tersebut termasuk dalam label sejarah FTMM.

Hasil yang diperoleh pada pertanyaan pertama sudah bisa menjawab sesuai dengan kemiripan dengan pertanyaan yang sebenarnya dari pattern yaitu 'Karya apa saja yang sudah dihasilkan FTMM?'. Namun kita menggunakan pertanyaan ’Karya yang pernah dihasilkan FTMM apa saja?’. Kemudian untuk pertanyaan kedua Chatbot tidak dapat menjawab karena score yang didapat lebih kecil dari kemiripan pada pattern 'Logo FTMM berwarna apa?'. Kemudian untuk pertanyaan terakhir yang berbeda, tanpa adanya ‘program studi’, chatbot dapat menjawab pertanyaan tersebut.





