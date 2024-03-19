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
