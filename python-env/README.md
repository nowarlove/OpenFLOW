<div align = center>

# Python Virtual Enviroment

![py](https://www.dataquest.io/wp-content/uploads/2022/01/python-virtual-envs1.webp)


</div>

Seperti namanya, Virtual Environment adalah sebuah ruang lingkup virtual yang terisolasi dari dependencies utama. Virtual Environment sangat berguna ketika kita membutuhkan dependencies yang berbeda-beda antara project satu dengan lainnya yang berjalan pada satu system operasi yang sama.

## Instalasi

### Untuk dapat menginstalkan, ada beberapa yang di butuhkan:

- python3
- python3-venv

### Langkah-langkah

1. Yang pertama anda harus menginstalkan terlebih dahulu python3-venv

    - ``` > sudo apt install python3-venv ```
2. Lalu buatlah folder baru bebas dengan nama apapun
    - ``` > mkdir python-env ``` # misalnya saya disini pakai nama ini
3. Lalu installkan komponen yang akan di gunakan pada folder tadi
    - ``` > python3 -m venv python-env/ ```
4. Tunggu hingga selesai, lalu coba aktifkan dengan command
    - ``` > source python-env/bin/active ```
5. Untuk menonaktifkan cukup ketikkan perintah
    - ``` > deactive ```
