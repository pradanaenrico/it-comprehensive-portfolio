# 📚 Portofolio IT Komprehensif - Enrico Pradana Antoni Putra

Dokumen ini memuat rangkuman detail teknis, arsitektur, serta cakupan pengembangan dari proyek-proyek IT yang pernah saya kerjakan baik secara profesional di industri maupun akademis.

---

## 📋 Daftar Proyek (1 - 10)

### 1. Aplikasi Internal & Operasional Perusahaan (Merak Jaya Group)
* **Perusahaan:** Merak Jaya Group *(Desember 2022 – Agustus 2026)*
* **Deskripsi:** Sistem aplikasi web internal terpadu dan aplikasi mobile untuk menunjang produktivitas harian di lingkungan *plant*.
* **Tech Stack:** PHP, Lumen, ReactJS, ExtJS, Oracle Database, MySQL, Android (Java), Git, Postman.
* **Fitur Utama / Tanggung Jawab:**
  * Mendesain dan mengembangkan arsitektur REST API berperforma tinggi menggunakan framework **Lumen**.
  * Pengembangan modul **Surat Jalan (SJ)** untuk pencatatan dan pelacakan logistik pengiriman.
  * Pengembangan modul **Slip Gaji** digital untuk karyawan.
  * Pemeliharaan dan optimasi kueri pada database **Oracle** dan **MySQL**.

### 2. Sistem Informasi Pendidikan (Think Indonesia)
* **Instansi/Klien:** Think Indonesia *(2021)*
* **Deskripsi:** Platform web manajemen sekolah untuk mempermudah administrasi akademik dan pengelolaan data sekolah.
* **Tech Stack:** CodeIgniter 3, MySQL, AdminLTE, JavaScript, Git.
* **Fitur Utama / Tanggung Jawab:**
  * Mengembangkan modul manajemen jadwal guru dan siswa secara dinamis.
  * Mengimplementasikan fitur pencatatan absensi digital.
  * Mengelola sistem *master data* akademik dan berkoordinasi langsung dengan *user* terkait kebutuhan fitur.

### 3. Aplikasi Pengenalan Anggota Tubuh & Gerak Tubuh (Android)
* **Jenis Proyek:** Proyek Akhir / Tugas Akhir Universitas Dinamika *(2019)*
* **Deskripsi:** Aplikasi edukasi berbasis seluler interaktif untuk anak-anak guna mengenal bagian tubuh dan gerakan dasar.
* **Tech Stack:** Android Native (Java), SQLite / Local Storage.
* **Fitur Utama:**
  * Fitur pengenalan anatomi anggota tubuh anak dengan panduan suara/audio.
  * Simulasi animasi pengenalan gerak tubuh.
  * Fitur kuis edukatif interaktif untuk evaluasi pembelajaran anak.

### 4. Real-time Silo Sensor Monitoring & Reporting System
* **Deskripsi:** Sistem monitoring berskala industri untuk melacak telemetri fisik volume material pada silo secara *real-time*.
* **Tech Stack:** ExtJS (Frontend), PHP (Backend API), InfluxDB (Time-Series DB), Oracle DB (Master Data).
* **Fitur Utama / Tanggung Jawab:**
  * **Penyusunan Hybrid Database Architecture:** Mengintegrasikan skema relasional Oracle DB dengan InfluxDB untuk mencegah *bottleneck* I/O server[cite: 1].
  * **Visualisasi Data & Historikal Tren:** Membangun antarmuka manajemen menggunakan framework ExtJS guna menampilkan data grafik fluktuasi isi silo dan tabel riwayat analitik secara dinamis[cite: 1].
  * **Optimasi Query Rentang Waktu:** Merancang dan melakukan tuning pada REST endpoint berbasis PHP untuk memproses penarikan data telemetri historis dalam rentang waktu yang masif tanpa mengorbankan waktu respon aplikasi[cite: 1].

### 5. Real-time Vehicle Maintenance Dashboard
* **Deskripsi:** Dashboard manajemen dan pemeliharaan armada logistik perusahaan berkinerja tinggi, mengandalkan transmisi data instan melalui arsitektur WebSocket serta sistem *caching in-memory*.
* **Tech Stack:** Next.js, Tailwind CSS, Material UI, Express.js, Redis Cache, Oracle DB, uWebSockets / Socket.io.
* **Fitur Utama / Tanggung Jawab:**
  * **Mekanisme Scheduler & Redis Caching:** Membangun *background scheduler* untuk melakukan *pre-fetching* data riwayat perbaikan kendaraan dari Oracle DB ke Redis secara berkala guna mengoptimalkan kecepatan pembacaan data di frontend[cite: 1].
  * **Data Streaming berlatensi Rendah:** Mengintegrasikan uWebSockets / Socket.io pada backend Express.js untuk melakukan *push-update* data status perawatan armada ke antarmuka klien secara instan tanpa memicu *reload* halaman[cite: 1].
  * **Desain Modern UI/UX Component:** Menyusun tata letak dasbor yang adaptif menggunakan paduan Tailwind CSS dan visualisasi statis komponen Material UI demi mempermudah operator logistik melakukan monitoring[cite: 1].

### 6. Prospect Customer Application (Sales Mobile Suite)
* **Deskripsi:** Aplikasi mobile native Android untuk memfasilitasi aktivitas lapangan tim sales/marketing saat melakukan kunjungan ke pelanggan (prospek penawaran, pengajuan limit kredit baru, hingga pencatatan repeat order).
* **Tech Stack:** Java (Android Native), Lumen Framework, REST API, Oracle / MySQL, GPS & Camera API.
* **Fitur Utama / Tanggung Jawab:**
  * **Alur Validasi Lokasi Kunjungan:** Mengembangkan fitur verifikasi kunjungan kerja tim sales berbasis GPS data koordinat, integrasi kamera untuk bukti fisik check-in di lokasi, dan enkripsi data formulir sebelum dikirim[cite: 1].
  * **Sinkronisasi Data Dinamis:** Membangun backend service menggunakan Lumen API untuk mengamankan proses unggah file gambar dokumen fisik, data leads, dan mutasi status prospek ke database pusat[cite: 1].

### 7. Prospect Collector Application (Collection Mobile Suite)
* **Deskripsi:** Solusi mobile keuangan lapangan yang terintegrasi untuk membantu divisi collector memetakan daftar piutang dagang, melakukan pelacakan penagihan langsung ke nasabah, serta mengunci rekonsiliasi data pembayaran.
* **Tech Stack:** Java (Android Native), Lumen Framework, SQLite / Local Storage, REST API.
* **Fitur Utama / Tanggung Jawab:**
  * **Manajemen Invoice Terintegrasi:** Menyusun tata letak antarmuka data tagihan jatuh tempo yang disinkronkan langsung dari ERP pusat ke aplikasi perangkat mobile collector[cite: 1].
  * **Payment Logging & Security Check-in:** Mengimplementasikan pencatatan mutasi transaksi pembayaran di tempat (tunai/transfer) yang diikat dengan validasi check-in foto lokasi dan penutupan log saat sales menekan tombol checkout[cite: 1].

### 8. End-to-End Enterprise Order to Logistics System (O2L)
* **Deskripsi:** Sistem ERP web terpadu yang memayungi seluruh rangkaian transaksi pasca-kunjungan sales secara sekuensial dan terorganisir untuk memproses administrasi bisnis dari hulu ke hilir bisnis.
* **Tech Stack:** HTML5, Native JavaScript, jQuery, Bootstrap, PHP Backend, Relational DB.
* **Fitur Utama / Tanggung Jawab:**
  * **Otomasi Sekuensial Alur Dokumen Transaksi:**
    * *Quotation:* Penyusunan modul kalkulasi penawaran harga jual barang[cite: 1].
    * *Sales Order (SO):* Konversi quotation disetujui menjadi dokumen SO formal[cite: 1].
    * *Schedule Produksi:* Integrasi pemetaan data SO ke dalam jadwal produksi lantai pabrik (*plant*)[cite: 1].
    * *Surat Jalan (SJ):* Penerbitan otomatis berkas legalitas pengiriman logistik[cite: 1].
  * **Optimasi Data-Entry Multi-Baris:** Memaksimalkan manipulasi DOM secara *real-time* via Native JavaScript dan jQuery untuk menangani formulir input barang berskala besar tanpa adanya *delay rendering*[cite: 1].

### 9. Intelligent Chatbot Integration (Telegram Bot & LLM Engine)
* **Deskripsi:** Aplikasi agen Generative AI interaktif berbasis *asynchronous event loop* di Python yang menghubungkan platform pesan instan Telegram dengan LLM kelas enterprise.
* **Tech Stack:** Python, Groq Cloud API, Llama 3.3 (70B Versatile), python-telegram-bot, Asynchronous Loops.
* **Fitur Utama / Tanggung Jawab:**
  * **Advanced Prompt Engineering:** Menyusun struktur berkas instruksi internal (*System Prompt*) tingkat lanjut untuk mengatur kendali persona AI agar luwes namun tetap akurat[cite: 1].
  * **Context Window Management:** Mengembangkan mekanisme *in-memory session chat history* dengan teknik *array slicing* untuk membatasi 10 riwayat pesan teratas, menghemat token, dan menjaga memori percakapan[cite: 1].
  * **Conditional Context Injection:** Menyuntikkan logika gerbang data dinamis berbasiskan Telegram User ID unik pengguna untuk membedakan perlakuan dan latar belakang respon otomatis bot[cite: 1].

### 10. AI-Powered Conversational Point of Sales (POS) & Analytics System
* **Deskripsi:** Inovasi sistem Point of Sales (POS) berbasis percakapan (*Conversational Commerce*) untuk mendigitalisasi operasional UMKM, dibangun menggunakan arsitektur *event-driven* Node.js.
* **Tech Stack:** Node.js, @whiskeysockets/baileys, better-sqlite3, SheetJS (xlsx), Generative AI Analytics.
* **Fitur Utama / Tanggung Jawab:**
  * **State-Machine Router UI Menu:** Mengembangkan alur *parsing* teks perintah kasir interaktif untuk manajemen Master User, Master Produk, modul Tambah Stok, dan fungsi kasir[cite: 1].
  * **Embedded High-Performance DB (SQLite):** Menggunakan *database engine* `better-sqlite3` untuk penulisan data transaksi kilat secara lokal tanpa resiko *file locking*[cite: 1].
  * **AI Business Insight & Analytics:** Mengintegrasikan data kompilasi bulanan dengan model AI untuk memberikan ulasan bisnis strategis, pemetaan produk terlaris (*fast-moving*), dan pengelolaan stok otomatis[cite: 1].

---
*Kembali ke Profil Utama: [github.com/pradanaenrico](https://github.com/pradanaenrico)*
