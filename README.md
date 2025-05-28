# 📚 Bookshelf API

Bookshelf API adalah proyek backend sederhana yang dibangun menggunakan framework **Hapi.js** untuk mengelola data buku. 

## ✨ Fitur

### ✅ Fitur Wajib
- Menyimpan buku baru
- Menampilkan seluruh buku
- Menampilkan detail buku berdasarkan ID
- Mengubah data buku berdasarkan ID
- Menghapus buku berdasarkan ID

### ⚙️ Fitur Opsional
- Filter buku berdasarkan query:
  - `?name=` : Mencari buku berdasarkan nama (tidak case-sensitive)
  - `?reading=` : Filter buku yang sedang dibaca (`1`) atau tidak (`0`)
  - `?finished=` : Filter buku yang sudah selesai (`1`) atau belum (`0`)
- Menggunakan **ESLint** dengan style guide dan bebas dari error
- Menyediakan script `start` untuk menjalankan server

## 📁 Struktur Proyek
````
src/
├── books.js # Data penyimpanan buku (in-memory)
├── handler.js # Logic untuk menangani setiap route
├── routes.js # Daftar semua endpoint (routing)
└── server.js # Konfigurasi server Hapi
````
## 🚀 Cara Menjalankan
1. Clone repository
2. npm install
3. npm run start
4. Server akan berjalan di http://localhost:9000

## 🧪 Testing API
- POST /books
- GET /books
- GET /books/{id}
- PUT /books/{id}
- DELETE /books/{id}
