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
