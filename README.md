<details>
<Summary><b>Tugas 5</b></Summary>

### Jelaskan apa itu widget tree pada Flutter dan bagaimana hubungan parent-child (induk-anak) bekerja antar widget.
Widget tree pada Flutter adalah struktur hierarkis yang menggambarkan bagaimana widget-widget dalam aplikasi Flutter diatur dan saling berhubungan. Setiap widget dalam Flutter adalah elemen dasar dari antarmuka pengguna, dan widget-tree menggambarkan bagaimana widget-widget tersebut disusun satu sama lain.

### Sebutkan semua widget yang kamu gunakan dalam proyek ini dan jelaskan fungsinya.
1. MaterialApp: Widget ini adalah root dari aplikasi Flutter yang menyediakan tema dan navigasi dasar.
2. Scaffold: Widget ini menyediakan struktur dasar untuk halaman aplikasi, termasuk app bar, body, dan drawer.
3. AppBar: Widget ini digunakan untuk menampilkan bar di bagian atas layar yang biasanya berisi judul dan tindakan.
4. Drawer: Widget ini menyediakan panel samping yang dapat digeser untuk menampilkan menu navigasi.
5. ListView: Widget ini digunakan untuk menampilkan daftar gulir dari item-item.
6. Card: Widget ini digunakan untuk menampilkan informasi dalam bentuk kartu dengan bayangan dan sudut melengkung
7. Icon: Widget ini digunakan untuk menampilkan ikon grafis.
8. Text: Widget ini digunakan untuk menampilkan teks di layar.
9. MyHomePage: Widget yang adalah halaman utama dari aplikasi yang dibuat.
10. ItemHomepage: Kelas yang merepresentasikan item dalam daftar menu.
11. Padding: Widget ini digunakan untuk memberikan ruang di sekitar widget lain.
12. Center: Widget ini digunakan untuk memusatkan widget anak di dalamnya.
13. Column: Widget ini digunakan untuk mengatur widget anak secara vertikal.
14. Row: Widget ini digunakan untuk mengatur widget anak secara horizontal.
15. GestureDetector: Widget ini digunakan untuk mendeteksi interaksi pengguna seperti ketukan.
16. Navigator: Widget ini digunakan untuk mengelola tumpukan halaman dan navigasi antar halaman.


### Apa fungsi dari widget MaterialApp? Jelaskan mengapa widget ini sering digunakan sebagai widget root.
Widget MaterialApp adalah widget yang menyediakan struktur dasar untuk aplikasi Flutter yang mengikuti prinsip desain Material Design. Widget ini sering digunakan sebagai widget root karena menyediakan berbagai fitur penting seperti tema, navigasi, dan manajemen rute yang memudahkan pengembangan aplikasi. Dengan menggunakan MaterialApp, kita dapat dengan mudah mengatur tampilan dan perilaku aplikasi sesuai dengan standar desain yang konsisten.

### Jelaskan perbedaan antara StatelessWidget dan StatefulWidget. Kapan kamu memilih salah satunya?
StatelessWidget adalah widget yang tidak memiliki keadaan yang dapat berubah selama siklus hidupnya. Widget ini hanya bergantung pada data yang diberikan saat pembuatan dan tidak dapat memperbarui dirinya sendiri. StatelessWidget cocok digunakan untuk elemen UI yang statis dan tidak memerlukan interaksi atau perubahan data. StatefulWidget, di sisi lain, adalah widget yang memiliki keadaan yang dapat berubah selama siklus hidupnya. Widget ini dapat memperbarui dirinya sendiri berdasarkan interaksi pengguna atau perubahan data. StatefulWidget cocok digunakan untuk elemen UI yang dinamis dan memerlukan interaksi atau perubahan data.

### Apa itu BuildContext dan mengapa penting di Flutter? Bagaimana penggunaannya di metode build?
BuildContext adalah objek yang menyediakan informasi tentang lokasi widget dalam hierarki widget. BuildContext penting di Flutter karena memungkinkan widget untuk mengakses informasi tentang lingkungan sekitarnya, seperti tema, ukuran layar, dan navigasi. Dalam metode build, BuildContext digunakan untuk mendapatkan referensi ke widget induk atau untuk mengakses data yang disediakan oleh widget lain dalam hierarki. Misalnya, BuildContext dapat digunakan untuk mendapatkan tema aplikasi atau untuk menavigasi ke halaman lain.

### Jelaskan konsep "hot reload" di Flutter dan bagaimana bedanya dengan "hot restart".
"Hot reload" di Flutter adalah fitur yang memungkinkan pengembang untuk melihat perubahan kode secara instan tanpa harus memulai ulang aplikasi. Dengan hot reload, perubahan pada kode sumber dapat diterapkan langsung ke aplikasi yang sedang berjalan, sehingga pengembang dapat dengan cepat melihat hasil perubahan tanpa kehilangan status aplikasi saat ini. Hot reload sangat berguna untuk mempercepat proses pengembangan dan debugging. "Hot restart", di sisi lain, adalah proses yang memulai ulang aplikasi dari awal, menghapus semua status dan data yang ada. Hot restart digunakan ketika perubahan kode memerlukan reset penuh aplikasi, seperti perubahan pada struktur widget atau inisialisasi ulang data. Hot restart memakan waktu lebih lama dibandingkan hot reload karena harus memulai ulang seluruh aplikasi.

</details>