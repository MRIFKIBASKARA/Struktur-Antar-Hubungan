# Jawaban Soal Struktur Antar Hubungan

## 1. Struktur Antar Hubungan dan Contohnya
Struktur antar hubungan adalah cara komponen komputer seperti **CPU, memori, dan perangkat I/O** berkomunikasi.  

**Komponen utama:**
- **Bus Sistem** → Jalur komunikasi antar komponen.  
- **CPU** → Mengolah data dan menjalankan program.  
- **Memori** → Menyimpan data dan instruksi.  
- **Perangkat I/O** → Menghubungkan komputer dengan perangkat luar.  

**Contoh:**  
CPU mengambil data dari memori melalui bus, mengolahnya, lalu mengirim hasilnya kembali ke memori atau perangkat I/O.  

---

## 2. Penyebab Penurunan Kinerja Jika Terlalu Banyak Perangkat di Bus  
Jika terlalu banyak perangkat terhubung ke bus, kinerja menurun karena:  

1. **Bus jadi sibuk** → Banyak perangkat berbagi jalur komunikasi.  
2. **Waktu tunggu meningkat** → CPU dan perangkat lain harus antre.  
3. **Kecepatan transfer turun** → Bandwidth terbatas.  
4. **Tabrakan data** → Jika banyak perangkat mengirim data bersamaan, terjadi benturan yang memperlambat sistem.  
5. **Sistem lebih rumit** → Manajemen akses bus butuh waktu tambahan.  

---

## 3. Mengapa Perangkat Prioritas 16 Bisa Punya Waktu Tunggu Lebih Singkat?  
Biasanya, perangkat dengan prioritas tinggi mendapat akses lebih dulu. Namun, prioritas 16 (rendah) bisa punya waktu tunggu lebih singkat jika:  

1. **Jarang dipakai** → Tidak sering meminta akses, jadi saat butuh bisa langsung masuk.  
2. **Sistem seimbang** → Jika perangkat prioritas tinggi cepat selesai, prioritas rendah bisa langsung masuk.  

**Kapan Ini Tidak Berlaku?**  
- Jika **perangkat prioritas tinggi selalu sibuk**, prioritas rendah akan menunggu lama.  
- Jika sistem memakai **round-robin (giliran bergantian)**, prioritas tidak lagi berpengaruh.  
- Jika **beban kerja meningkat**, perangkat prioritas tinggi bisa mendominasi bus.  
