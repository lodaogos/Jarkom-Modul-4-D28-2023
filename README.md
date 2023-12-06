# Jarkom-Modul-4-D28-2023

## Pembagian Subnet

Pembagian subnet dapat dilihat sebagai berikut.

![image](https://github.com/lodaogos/Jarkom-Modul-4-D28-2023/assets/115076652/48b4a731-8fdd-490e-82c3-ecd926a6ab72)

## VLSM Tree
Untuk memudahkan dalam membagi perhitungan VLSM, kami menggunakan Tree terlebih dahulu.

![VLSM](https://github.com/lodaogos/Jarkom-Modul-4-D28-2023/assets/34641833/cc8e9360-6e70-4171-b6ed-c2420fc5c440)

## Pembagian Perhitungan VLSM
Setelah itu, kami bisa melakukan pembagian perhitungan untuk VLSM.

![VLSM - PEMBAGIAN NETWORK](https://github.com/lodaogos/Jarkom-Modul-4-D28-2023/assets/34641833/d33aaaeb-c93c-4c5c-a815-7e014ba35455)

## Konfigurasi CPT
Setelah menentukan semua subnet, kita bisa buka router node Aura dan isi IP berdasarkan arah eth. Contohnya, Aura ke Frieren melalui Fa1/0, maka Frieren kembali ke Aura melalui Fa0/0.

![VLSM - CONFIG AURA](https://github.com/lodaogos/Jarkom-Modul-4-D28-2023/assets/34641833/bb4c28de-c7b3-4199-94d4-d71674914034)

![VLSM - CONFIG FRIEREN](https://github.com/lodaogos/Jarkom-Modul-4-D28-2023/assets/34641833/b7d5ca26-9135-4b19-8620-05798ca01cd0)

Lakukan hal yang sama kepada node-node lain.

## Routing CPT
Untuk menghubungkan semua subnet, kita bisa melakukan routing dengan membuka node router, lalu pilih Routing -> Static. Setelah itu Network diisi dengan IP yang dituju, Mask diisi dengan Netmask IP tersebut. Lalu, Next Hop diisi dengan node router terdekat yang menjadi jembatan. Untuk routing mundur (menuju Aura) Network dan Mask diisi dengan 0.0.0.0.

![VLSM - ROUTING AURA](https://github.com/lodaogos/Jarkom-Modul-4-D28-2023/assets/34641833/103ef249-7797-44fb-a7e3-3e5ac9d11d42)

## Pembagian Perhitungan CIDR

Dari subnet tersebut kita bisa bagi gabungkan subnet satu per satu hingga menjadi sebuah subnet besar seperti berikut ini.

![image](https://github.com/lodaogos/Jarkom-Modul-4-D28-2023/assets/115076652/f11affc7-d23a-4c5d-8a2b-80128fea19c3)

## Penggabungan CIDR

Kemudian kita bisa menghitung netmask total deengan menggabungkan masing-masing subnet hingga menjadi subnet besar.

![image](https://github.com/lodaogos/Jarkom-Modul-4-D28-2023/assets/115076652/9b3cf125-bda1-4b22-b50d-5db27184a946)

![image](https://github.com/lodaogos/Jarkom-Modul-4-D28-2023/assets/115076652/45d96638-e23e-46c6-9d73-6cd163c17d3d)

## Pohon CIDR

Dari hasil subnet mask yang didapatkan, kita bisa menghitung pembagian IP dengan pohon berdasarkan subnet tersebut.

![image](https://github.com/lodaogos/Jarkom-Modul-4-D28-2023/assets/115076652/d396e926-ee00-4ccb-b6f2-167a1cba6db3)


## Pembagian IP CIDR

Kemudian kita bisa tulis IP untuk masing-masing subnet tersebut.

![image](https://github.com/lodaogos/Jarkom-Modul-4-D28-2023/assets/115076652/c1eb7055-e2c8-4405-9156-0a78ced65092)
