​1. Analisis Materi: Array vs List. 
​Bayangkan Anda memiliki kotak penyimpanan:
​Array (Lemari Besi): Ukurannya tetap (misal: hanya 5 laci). Anda tidak bisa menambah laci baru di tengah jalan. Sangat hemat tempat dan cepat jika Anda hanya perlu mengambil barang dari laci tertentu.  
​List (Tas Belanja): Ukurannya fleksibel. Bisa membesar atau mengecil secara otomatis. Namun, ia memakan lebih banyak tempat di memori karena selalu menyiapkan ruang kosong ekstra untuk berjaga-jaga. 
 
Ringkasan Aturan The Game of Life. 
​Ini adalah simulasi sel hidup/mati pada papan kotak-kotak dengan 4 aturan utama:  
​Tetap Hidup: Sel hidup dengan 2 atau 3 tetangga tetap hidup.  
​Kesepian: Sel hidup dengan < 2 tetangga akan mati.  
​Kepadatan: Sel hidup dengan > 3 tetangga akan mati.  
​Kelahiran: Sel mati dengan tepat 3 tetangga akan jadi hidup.  

​2. Implementasi Kode Sederhana
​Karena Python secara bawaan tidak memiliki array murni seperti di bahasa C++, kita sering menggunakan List. Namun, kita akan mensimulasikan logika "Array" (ukuran tetap).
