# Routing and monitoring

Program controller : shortest-path routing, monitoring node and link status NetworkX integration

![s-lf](/practice/img/spine-leaf%20architecture.png)

## Routing

1. Hal yang perlu di siapkan
    - Topologi jaringan
    - Komputasi jalur routing antar switch
    - flow rule untuk jalur routing

2. Studi kasus
    - Topologi data center dengan skema [leaf and spine](/architecture/spine-leaf%20architecture.md)
    - terdiri dari akses switch dan core switch
    - studi kasus 1 : pengiriman via controller
    - studi kasus 2 : pengiriman via shortest path routing

## studi kasus 1 - routing via controller
1. skenario :
- ARP paket dari host dikirim ke controller oleh access switch
- Controller akan mengirim paket ke semua access switch yang lain

2. implementasi :
- Controller memonitor topologi jaringan
- Controller akan menginstallkan flow rule static untuk mengirim paket ke controller di setiap access switch
- Controller akan meneruskan paket tersebut ke access switch selain access switch pengirim

## Pengujian

1. Jalankan aplikasi controller dengan perintah
    - ``` > ryu-manager simpleswitchL3.py```

1. Jalankan aplikasi controller dengan perintah
    - ``` > ryu-manager simpleswitchL3.py```

1. Jalankan aplikasi controller dengan perintah
    - ``` > ryu-manager simpleswitchL3.py```

1. Jalankan aplikasi controller dengan perintah
    - ``` > ryu-manager simpleswitchL3.py```

1. Jalankan aplikasi controller dengan perintah
    - ``` > ryu-manager simpleswitchL3.py```

1. Jalankan aplikasi controller dengan perintah
    - ``` > ryu-manager simpleswitchL3.py```

1. Jalankan aplikasi controller dengan perintah
    - ``` > ryu-manager simpleswitchL3.py```
