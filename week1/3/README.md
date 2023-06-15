# ezqlite - SQLite Injection

> It's just a simple website, nothing strange right?

## About this challenge

Terlihat sebuah website sederhana untuk mencari lagu yang diinginkan.



Ketikkan sesuatu pada kueri lalu situs akan menampilkan lima lagu yang judulnya mengandung string pada kueri, diurutkan dari yang memegang peringkat teratas.


Disediakan pula file `app.py`. Di sinilah mulai terungkap petunjuknya.



Pada fungsi `filter_words()` terdapat kerentanan. Fungsi ini tidak dapat menghapus substring `/*` dan `*/` pada kueri yang dimasukkan user. Jika kueri yang dimasukkan adalah `'/*'` maka saksikan kejutannya.



Ya, muncullah daftar 100 lagu yang terdapat pada database `songs.db`.
