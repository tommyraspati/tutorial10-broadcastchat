# Tutorial 10 - Advanced Programming - Brodcast Chat Application

## Original Code

<img src="images/tutorial10-server.png">
<img src="images/tutorial10-client1.png">
<img src="images/tutorial10-client2.png">
<img src="images/tutorial10-client3.png">



Untuk menjalan server saya menggunakan perintah `cargo run --bin server`. Untuk menjalankan client saya menggunakan perintah `cargo run --bin client`. Ketika pengguna berinteraksi dengan WebSocket, baik sebagai klien atau server, pesan yang dikirim oleh salah satu klien akan diteruskan oleh server ke semua klien yang terhubung. Ini menciptakan efek "broadcast" di mana pesan yang dikirim oleh satu klien akan diterima oleh semua klien yang terhubung.

## Modifying the websocket port

<img src="images/tutorial102.2.png">

Untuk memastikan koneksi yang lancar, penting untuk memastikan bahwa kedua sisi, baik client maupun server, menggunakan port yang sama. Jika port yang digunakan oleh client dan server berbeda, koneksi tidak akan berhasil karena client akan mencoba terhubung ke server menggunakan port yang berbeda dari yang diharapkan.

