​1. Analisis File: Array vs. List dan Game of Life
​Terdapat tiga poin utama yang dibahas:

​A. Perbedaan Array dan List (Python)
​Meskipun terlihat mirip, keduanya memiliki karakteristik berbeda:
• ​Array: Ukurannya tetap (fixed). Lebih efisien dalam penggunaan memori karena tidak ada ruang ekstra yang terbuang. Cocok jika jumlah data sudah diketahui sejak awal.  
• ​List: Ukurannya dinamis (bisa bertambah/berkurang). Lebih fleksibel dengan banyak operasi seperti menambah dan menghapus elemen, namun memakan lebih banyak memori.  

B. Struktur Data ADT Array
​Karena Python tidak memiliki array primitif seperti bahasa lain (C++ atau Java), kita mendefinisikan Abstract Data Type (ADT) Array. Operasi dasarnya meliputi:  
• ​Array(size): Membuat tempat penyimpanan.  
• ​getitem(index) & setitem(index, value): Membaca dan mengisi data.  
• ​length(): Mengetahui kapasitas total.  

​C. Game of Life
​Ini adalah simulasi sel yang hidup atau mati berdasarkan jumlah tetangganya (8 sel di sekitarnya).  
•​ Tetangga < 2: Mati (kesepian).  
• ​Tetangga 2 atau 3: Tetap hidup.  
• ​Tetangga > 3: Mati (overpopulasi).  
• ​Tetangga pas 3 (pada sel mati): Jadi hidup (kelahiran).

2. Penjelasan Logika Implementasi
​Dalam membuat simulasi ini, kita menerapkan teori Array dan aturan Game of Life sebagai berikut:

A. ​Pembuatan Papan (Inisialisasi):
• ​Kita menggunakan struktur array karena ukurannya tetap dan tidak berubah saat program berjalan.  
• ​Program membuat grid sesuai nilai size (baris dan kolom), di mana setiap elemen awalnya atau bernilai None.  

B. ​Mengatur Posisi Awal:
• ​Kita memasukkan organisme hidup ke dalam koordinat tertentu menggunakan operasi setitem.  
• ​Status "1" berarti hidup, dan "0" berarti mati.

C. ​Siklus Kehidupan (Generasi):
• ​Untuk setiap sel, program mengecek 8 tetangga di sekelilingnya (atas, bawah, kiri, kanan, dan diagonal).  
• ​Aturan Kematian: Jika sel hidup terlalu sendirian (0-1 tetangga) atau terlalu ramai (≥4 tetangga), ia akan mati.  
• ​Aturan Bertahan: Jika sel hidup memiliki 2 atau 3 tetangga, ia tetap hidup di generasi berikutnya.  
• ​Aturan Kelahiran: Jika ada sel mati yang dikelilingi tepat 3 tetangga hidup, sel itu "lahir" menjadi hidup.  

D. Pembaruan Serentak:
• ​Sangat penting untuk tidak langsung mengubah papan yang sedang dihitung. Kita membuat "papan bayangan" (array baru) untuk menyimpan hasil perhitungan.  
• ​Setelah semua sel selesai dihitung, papan lama diganti dengan papan baru secara utuh. Ini menciptakan efek "generasi" yang berubah bersamaan.
