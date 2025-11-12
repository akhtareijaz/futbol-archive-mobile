<details>
<Summary><b>Tugas 7</b></Summary>

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
BuildContext adalah objek yang menyediakan informasi tentang lokasi widget dalam hierarki widget. BuildContext penting di flutter karena memungkinkan widget untuk mengakses informasi tentang lingkungan sekitarnya, seperti tema, ukuran layar, dan navigasi. Dalam metode build, BuildContext digunakan untuk mendapatkan referensi ke widget induk atau untuk mengakses data yang disediakan oleh widget lain dalam hierarki. Misalnya, BuildContext dapat digunakan untuk mendapatkan tema aplikasi atau untuk menavigasi ke halaman lain.

### Jelaskan konsep "hot reload" di Flutter dan bagaimana bedanya dengan "hot restart".
"Hot reload" di Flutter adalah fitur yang memungkinkan pengembang untuk melihat perubahan kode secara instan tanpa harus memulai ulang aplikasi. Dengan hot reload, perubahan pada kode sumber dapat diterapkan langsung ke aplikasi yang sedang berjalan, sehingga pengembang dapat dengan cepat melihat hasil perubahan tanpa kehilangan status aplikasi saat ini. Hot reload sangat berguna untuk mempercepat proses pengembangan dan debugging. "Hot restart", di sisi lain, adalah proses yang memulai ulang aplikasi dari awal, menghapus semua status dan data yang ada. Hot restart digunakan ketika perubahan kode memerlukan reset penuh aplikasi, seperti perubahan pada struktur widget atau inisialisasi ulang data. Hot restart memakan waktu lebih lama dibandingkan hot reload karena harus memulai ulang seluruh aplikasi.

</details>

<details>
<Summary><b>Tugas 8</b></Summary>

### Jelaskan perbedaan antara Navigator.push() dan Navigator.pushReplacement() pada Flutter. Dalam kasus apa sebaiknya masing-masing digunakan pada aplikasi Football Shop kamu?
Navigator.push() adalah metode yang digunakan untuk menambahkan halaman baru ke tumpukan navigasi tanpa menghapus halaman sebelumnya. Ini memungkinkan pengguna untuk kembali ke halaman sebelumnya menggunakan tombol kembali. Navigator.push() sebaiknya digunakan ketika pengguna perlu menavigasi ke halaman baru tetapi masih ingin memiliki kemampuan untuk kembali ke halaman sebelumnya, seperti saat menavigasi dari halaman utama ke halaman detail produk di aplikasi Football Shop.
Navigator.pushReplacement() adalah metode yang digunakan untuk menggantikan halaman saat ini dengan halaman baru, menghapus halaman sebelumnya dari tumpukan navigasi. Ini berarti pengguna tidak dapat kembali ke halaman sebelumnya setelah navigasi. Navigator.pushReplacement() sebaiknya digunakan ketika pengguna menyelesaikan suatu tindakan dan tidak perlu kembali ke halaman sebelumnya, seperti setelah menyelesaikan proses pembayaran di aplikasi Football Shop, di mana pengguna langsung diarahkan ke halaman konfirmasi tanpa perlu kembali ke halaman pembayaran.

### Bagaimana kamu memanfaatkan hierarchy widget seperti Scaffold, AppBar, dan Drawer untuk membangun struktur halaman yang konsisten di seluruh aplikasi?
Dalam membangun struktur halaman yang konsisten di seluruh aplikasi Football Shop, saya memanfaatkan hierarchy widget seperti Scaffold, AppBar, dan Drawer dengan cara berikut:
1. Scaffold: Saya menggunakan widget Scaffold sebagai kerangka dasar untuk setiap halaman dalam aplikasi. Scaffold menyediakan struktur yang konsisten dengan area untuk AppBar, body, dan Drawer, sehingga setiap halaman memiliki tata letak yang seragam.
2. AppBar: Saya menambahkan widget AppBar di dalam Scaffold untuk menampilkan judul halaman dan tindakan penting seperti ikon pencarian atau keranjang belanja. Dengan menggunakan AppBar yang konsisten di setiap halaman, pengguna dapat dengan mudah mengenali dan menavigasi aplikasi.
3. Drawer: Saya menyertakan widget Drawer di dalam Scaffold untuk menyediakan menu navigasi samping yang dapat diakses dari setiap halaman. Drawer berisi tautan ke berbagai bagian aplikasi, seperti kategori produk, profil pengguna, dan pengaturan. Dengan menggunakan Drawer yang konsisten, pengguna dapat dengan mudah berpindah antar halaman tanpa kehilangan konteks.

### Dalam konteks desain antarmuka, apa kelebihan menggunakan layout widget seperti Padding, SingleChildScrollView, dan ListView saat menampilkan elemen-elemen form? Berikan contoh penggunaannya dari aplikasi kamu.
Menggunakan layout widget seperti Padding, SingleChildScrollView, dan ListView memiliki beberapa kelebihan dalam konteks desain antarmuka:
1. Padding: Widget Padding memungkinkan saya untuk menambahkan ruang di sekitar elemen-elemen form, sehingga elemen-elemen tersebut tidak terlalu berdekatan dan lebih mudah dibaca. Contohnya, saya menggunakan Padding di sekitar teks input dan tombol submit di halaman checkout aplikasi Football Shop untuk memberikan jarak yang nyaman bagi pengguna.
2. SingleChildScrollView: Widget SingleChildScrollView memungkinkan konten form yang panjang untuk digulir, sehingga pengguna dapat mengakses semua elemen form tanpa terpotong. Contohnya, saya menggunakan SingleChildScrollView di halaman pendaftaran pengguna untuk memastikan bahwa semua bidang input dapat diakses meskipun layar perangkat memiliki ukuran terbatas.
3. ListView: Widget ListView memungkinkan saya untuk menampilkan daftar elemen form yang dapat digulir dengan efisien. Contohnya, saya menggunakan ListView untuk menampilkan daftar produk di halaman kategori, sehingga pengguna dapat dengan mudah menelusuri dan memilih produk yang mereka inginkan.

### Bagaimana kamu menyesuaikan warna tema agar aplikasi Football Shop memiliki identitas visual yang konsisten dengan brand toko?
1. Menggunakan ThemeData: Saya menggunakan ThemeData di dalam widget MaterialApp untuk mengatur warna tema aplikasi secara keseluruhan. Saya menetapkan warna primer, sekunder, latar belakang dengan warna yang ditentukan
2. Konsistensi di seluruh aplikasi: Saya memastikan bahwa warna tema digunakan secara konsisten di seluruh aplikasi, termasuk di AppBar, tombol, ikon, dan elemen UI lainnya. Hal ini membantu memperkuat identitas visual brand toko.

</details>