# Cara-Mengatasi-fatal-the-remote-end-hung-up-unexpectedlyMiB-58.00-KiB-s-fatal-early-EOF


Biasanya ketika akan install ccminer kita akan mengunduhnya dengan cara git clone --single-branch -b ARM https://github.com/monkins1010/ccminer.git . 

Namun ketika di tengah perjalanan mengunduh ccminer, lalu ada notifikasi eror sebagai berikut :

 - [ ] fatal: the remote end hung up unexpectedlyMiB | 58.00 KiB/s 
 - [ ] fatal: early EOF 
 - [ ] fatal: index-pack failed

Solusi nya adalah, ketika sebelum kita melakukan unduhan, maka sebaiknya kita kasih perintah dulu sebelum mengunduh.

Berikut adalah perintahnya (tulis perbaris, lalu enter, dan seterusnya) :

 - [ ] git init
 - [ ] git config http.postBuffer 524288000

Setelah itu kita lakukan proses unduh seperti biasanya melalui perintah git clone --single-branch -b ARM https://github.com/monkins1010/ccminer.git
Jika hal diatas masih saja terjadi, solusi paling gampang adalah kita mendownload langsung file zip ccminer nya ke komputer kita. Setelah terdownload ke komputer kita ekstrak di komputer lokal kita, lalu rename folder nya menjadi ccminer, setelah itu kita upload ke root STB nya menggunakan mobaexterm ataupun file manager lainnya. Saya lebih nyaman pake mobaexterm.
