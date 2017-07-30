## Panduan Kontribusi

Pada laman ini akan dijelaskan secara teknis untuk berkontribusi di repositori Lumbung BGLI. 

## 1. Git
Repositori Lumbung BGLI menggunakan Git sebagai aplikasi manajemen versi dan alat kontribusi. 
Sedangkan media penyimpanan menggunakan layanan GitHub. Panduan lengkap bagaimana memulai menggunakan Git dan Github bisa membaca referensi berikut

* [Github Guides : Hello World](https://guides.github.com/activities/hello-world/)

## 2. Fork
Fork adalah metode membuat "Salinan" terhadap repositori di Github. 
Dengan _fork_ kamu akan memiliki salinan repositori dari repositori asli di akun github.

![Contoh Repositori Hasil Fork](gambar/Kontribusi-fork.png)

Untuk memulai berkontribusi, kamu akan menggunakan salinan repositori tersebut untuk menambah, mengedit atau melakukan perubahan lainya. 

## 3. Clone / Unduh ke Komputer
Untuk dapat mengedit di komputer secara luring, kamu harus melakukan *clone* (dengan asumsi sudah menginstall Git client di komputer masing masing)

### Contoh Clone Repositori ke komputer

Berikut adalah contoh penggunaan perintah Git CLI yang dapat digunakan melalui Terminal
```
git clone git@github.com:showcheap/lumbung.git

Cloning into 'lumbung'...
remote: Counting objects: 3, done.
remote: Total 3 (delta 0), reused 3 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.
```

## 4. Kontribusi
Setelah melakukan clone, kini kamu dapat menyunting berkas, membuat berkas atau direktori baru. Berikut ini contoh membuat berkas baru menggunakan editor *vim*

```
# Masuk ke direktori lumbung
cd lumbung
vim Bantuan.md
```

_*Catatan:* Editor vim hanyalah contoh, silahkan gunakan editor kesayangan kamu misal emacs, Visual Studio Code, Gedit, Geany, Notepad++, dlsb._

* Format penulisan menggunakan markdown, sehingga berkas yang dibuat menggunakan ekstensi `.md`
* Template Berkas markdown sedang kami susun untuk keperluan kontribusi selanjutnya

## 5. Push / Dorong
Setelah kamu melakukan perubahan pada repositori lokal, maka saatnya melakukan commit. Sertakan commit message dengan baik dan jelas, perubahan apa yang ada buat sehingga memudahkan moderator untuk meninjau kontribusi kamu.

### Contoh Pesan Commit
``` bash
# Tambahkan berkas tertentu ke dalam git 
git add Kontribusi.md

# Atau tambahkan semua berkas yang memiliki perubahan (berkas baru atau berkas yang telah disunting)
git add .

# Check Git Status
git status

On branch master
Your branch is up-to-date with 'origin/master'.
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	new file:   Kontribusi.md
```

# Kemudian commit
git commit -m "Penambahan laman Bantuan Kontribusi"

# Lakukan push ke repositori online (Github)
git push

Counting objects: 5, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 18.94 KiB | 0 bytes/s, done.
Total 5 (delta 0), reused 0 (delta 0)
To github.com:showcheap/lumbung.git
   f599355..909ce31  master -> master
```

## 6. Ajukan Pull Request
Setelah hasil suntingan kita terunggah ke repositori online Gitub, maka saatnya mengajukan Pull Request ke repo asli *[bgli/lumbung](https://github.com/bgli/lumbung)* dari repositori hasil fork (salinan) milik kamu *username_kamu/lumbung*.

![Tombol Pull Request](gambar/Kontribusi-pull-request.png)

Klik tombol *New Pull Request* untuk memulai mengajukan Pull Request

![Laman pengajuan Pull Request](gambar/Kontribusi-laman-pr.png)

Cuplikan layar di atas adalah contoh laman pada saat mengajukan pull request, perhatikan hal hal berikut ini sebelum mengajukan pull request

* Pastikan statusnya adalah *Able to merge*
* Pastikan *branch* sumber (milik kamu) dan *branch* tujuan sudah sesuai.

Kemudian klik tombol *Create Pull Request* untuk melanjutkan, tambahkan pesan tambahan (format markdown) untuk mempermudah moderator memahami perubahan / penambahan pada kontribusi kamu.

![Contoh Pesan Pull Request](gambar/Kontribusi-pesan-pr.png)

Lanjutkan dengan klik tombol *Create Pull Request* 

## 7. Tunggu Review Dari Moderator
Untuk menghindari hal hal yang tidak diinginkan, makan kontribusi melalui pull request akan melalui proses moderasi. Harap bersabar sampai kontribusi anda disetujui dan di _merge_ ke repositori utama lumbung. Untuk mempercepat proses moderasi, lakukan hal hal berikut ini:

* Pastikan menggunakan tata bahasa yang baik dan benar
* Gunakan pesan pull request yang jelas (jelaskan perubahan atau penambahan yang anda lakukan)
* Colek admin melalui [Grup Telegram BGLI](https://t.me/GNULinuxIndonesia)

## 8. Selamat & Terimakasih
Selamat dan terimakasih kami ucapkan kepada seluruh kontributor, semoga ilmu yang dibagikan dapat bermanfaat untuk kemajuan Teknologi khususnya Perangkat Lunak Bebas dan Terbuka di Indonesia.
