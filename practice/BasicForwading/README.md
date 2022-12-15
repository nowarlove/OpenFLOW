# Basic Forwading

## Hal-hal yang harus di persiapkan
1. [Mininet](/mininet/README.md)
2. [Ryu](/ryu/README.md)

![img](/practice/img/topo.png)

## Dasar-dasar OpenFlow

```Silahakan untuk memperiapkann program topologi dan program kontrolerny, yang mana nanti akan di jalankan bersamaan.```

dalam implementasi openflow sendiri ada beberapa hal yang perlu di perhatikan, atau dalam pembelajaran kali ini saya akan menyebutnya sebagai **KOMPONEN** yang dimana terbagi atas:

1. Controller
    - Bertugas Menginstalkan dan memonitoring Openflow rules pada setiap switch (data plane)
    - User dapat membuat aplikasi yang berjalan di atas controller untuk mengatur kerja switch
    - kita akan menggunakan [**Ryu-controller**](/ryu/README.md) yang berjalan di atas bahasa pemrograman python

2. Openflow Switch
    - Data plane yang bertugas untuk mengirim paket antar perangkat jaringan menggunakan OpenFlow rules
    - kita akan menggunakan **OpenVSwitch** << Ini sudah terinstall bersamaan dengan **mininet**

3. Simulasi jaringan
    - Mensimulasikan konfigurasi topologi dan flow rules pada percobaan jaringan
    - kita akan menggunakan [Mininet](/mininet/README.md)