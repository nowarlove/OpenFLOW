# Native Installation from Source

``` doct
This option works well for local VM, remote EC2, and native installation. It assumes the starting point of a fresh Ubuntu, Debian, or (experimentally) Fedora installation.

We strongly recommend more recent Ubuntu or Debian releases, because they include newer versions of Open vSwitch. (Fedora also includes recent OvS releases.)
```

## Kebutuhan

- GIT
- Python2 dan Python3 yang di installkan pada mesin yang sama
- Python updates-alternatives

## Tahap instalasi

**1.** Clone repository anda pada path yang anda inginkan

- ``` > git clone https://github.com/mininet/mininet ```

**2.** Masuk ke directory mininet yang telah anda clone

- ``` > cd mininet/ ```

**3.** lakukan git tag (untuk mengecek versi yang anda inginkan)

- ```> git tag```

**4.** lalu lakukan git checkout (saya menggunakan mininet-2.3.0)

- ``` > git checkout git checkout -b mininet-2.3.0 2.3.0  # or whatever version you wish to install ```

**5.** lalu keluar dari directory mininet tadi

- ``` > cd .. ```

**6.** Sebelum melakukan instalasi periksa file installer dan ubah beberapa baris code (saya selalu terkena masalah ini ketika saya akan menginstallkan mininet secara nativ di komputer saya)

- ``` pergi ke directory /mininet/util/install.sh ```
- ``` ubah baris 234 menjadi git clone git@github.com:mininet/openflow.git ```
- nb : alasan mengubahnya = asumsi saya, openflow telah melakukan migrasi repository sehingga, ketika menginstallkan. Kita tidak dapat melakukan clonning terhadap repo default yang ada di **install.sh**

**7.** Setelah itu lakukan penginstallan dengan mengetikkan perintah :

- ``` > /mininet/util/install.sh [tambahkan pilihan anda lihat di bawah] ```

  - ``` -a : digunakan untuk menginstallkan semua dependenci yang ada/akan di intallkan semua komponent yang ada ```
  
  - ``` -nfv : digunakan untuk menginstallkan beberapa komponen saja, diantaranya Mininet, Openflow dan OpenVSwitch saja. ```

**8.** Enjoy
