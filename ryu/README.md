<div align = center>

# **RYU**

</div>

```Ryu is a component-based software defined networking framework. Ryu provides software components with well defined API's that make it easy for developers to create new network management and control applications. Ryu supports various protocols for managing network devices, such as OpenFlow, Netconf, OF-config, etc. About OpenFlow, Ryu supports fully 1.0, 1.2, 1.3, 1.4, 1.5 and Nicira Extensions.```

## Langkah Penginstalan

Sebelum melakukan penginstalan, pastikan anda telah mempersiapkan beberapa hal di bawah ini :

- [Mininet](/mininet/README.md)
- [Python Virtual Enviroment](/python-env/README.md)

**1.** Setelah semuanya sudah lengkap, kita akan mengaktifkan virtual env python terlebih dahulu.

- ``` > source /python-env/bin/active ```

**2.** Setelah virtual env sudah aktif, maka terminal anda akan tampak seperti ini

![gmbr](/ryu/gmbr/src-actv.png)

**3.** Setelah mengaktifkan python env, masuk kedalam folder ryu, yang telah kita clone tadi

- ```> cd /ryu/```

**4**. Lalu kita installkan ryu tadi dengan perintah.

- ``` > pip install . ```
