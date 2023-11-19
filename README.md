# Jarkom-Modul-3-I08-2023

Nama Anggota | NRP
------------------- | --------------		
Mardhatillah Shevy Ananti | 5025211070
Kirana Alivia Enrico | 5025211190

## Node Configuration
Aura (Router + DHCP Relay)
```
auto eth0
iface eth0 inet dhcp

auto eth1
iface eth1 inet static
	address 192.232.1.1
	netmask 255.255.255.0

auto eth2
iface eth2 inet static
	address 192.232.2.1
	netmask 255.255.255.0

auto eth3
iface eth3 inet static
	address 192.232.3.1
	netmask 255.255.255.0

auto eth4
iface eth4 inet static
	address 192.232.4.1
	netmask 255.255.255.0
```

Himmel (DHCP Server)
```
auto eth0
iface eth0 inet static
	address 192.232.1.2
	netmask 255.255.255.0
	gateway 192.232.1.1
```

Heiter (DNS Server)
```
auto eth0
iface eth0 inet static
	address 192.232.1.3
	netmask 255.255.255.0
	gateway 192.232.1.1
```

Denken (Database Server)
```
auto eth0
iface eth0 inet static
	address 192.232.2.2
	netmask 255.255.255.0
	gateway 192.232.2.1
```

Eisen (Load Balancer)
```
auto eth0
iface eth0 inet static
	address 192.232.2.3
	netmask 255.255.255.0
	gateway 192.232.2.1
```

Revolte (Client)
```
auto eth0
iface eth0 inet dhcp
```

Ritcher (Client)
```
auto eth0
iface eth0 inet dhcp
```

Lawine (PHP Worker) - FIXED ADDRESS
```
auto eth0
iface eth0 inet static
	address 192.232.3.4
	netmask 255.255.255.0
	gateway 192.232.3.1
```

Linie (PHP Worker) - FIXED ADDRESS
```
auto eth0
iface eth0 inet static
	address 192.232.3.5
	netmask 255.255.255.0
	gateway 192.232.3.1
```

Lugner (PHP Worker) - FIXED ADDRESS
```
auto eth0
iface eth0 inet static
	address 192.232.3.6
	netmask 255.255.255.0
	gateway 192.232.3.1
```

Sein (Client)
```
auto eth0
iface eth0 inet dhcp
```

Stark (Client)
```
auto eth0
iface eth0 inet dhcp
```

Frieren (Laravel Worker) - FIXED ADDRESS
```
auto eth0
iface eth0 inet static
	address 192.232.4.4
	netmask 255.255.255.0
	gateway 192.232.4.1
```

Flamme (Laravel Worker) - FIXED ADDRESS
```
auto eth0
iface eth0 inet static
	address 192.232.4.5
	netmask 255.255.255.0
	gateway 192.232.4.1
```

Fern (Laravel Worker) - FIXED ADDRESS
```
auto eth0
iface eth0 inet static
	address 192.232.4.6
	netmask 255.255.255.0
	gateway 192.232.4.1
```

## Soal-0
Kali ini, kalian diminta untuk melakukan register domain berupa riegel.canyon.yyy.com untuk worker Laravel dan granz.channel.yyy.com untuk worker PHP mengarah pada worker yang memiliki IP [prefix IP].x.1.

### Explanation

## Soal-1
Lakukan konfigurasi sesuai dengan peta yang sudah diberikan.

### Explanation

## Soal-2
Client yang melalui Switch3 mendapatkan range IP dari [prefix IP].3.16 - [prefix IP].3.32 dan [prefix IP].3.64 - [prefix IP].3.80 

### Explanation

## Soal-3
Client yang melalui Switch4 mendapatkan range IP dari [prefix IP].4.12 - [prefix IP].4.20 dan [prefix IP].4.160 - [prefix IP].4.168 

### Explanation

## Soal-4
Client mendapatkan DNS dari Heiter dan dapat terhubung dengan internet melalui DNS tersebut 

### Explanation

## Soal-5
Lama waktu DHCP server meminjamkan alamat IP kepada Client yang melalui Switch3 selama 3 menit sedangkan pada client yang melalui Switch4 selama 12 menit. Dengan waktu maksimal yang dialokasikan untuk peminjaman alamat IP selama 96 menit 

### Explanation

## Soal-6
Pada masing-masing worker PHP, lakukan konfigurasi virtual host untuk website berikut dengan menggunakan php 7.3. 

### Explanation

## Soal-7
Kepala suku dari Bredt Region memberikan resource server sebagai berikut:
a. Lawine, 4GB, 2vCPU, dan 80 GB SSD.
b. Linie, 2GB, 2vCPU, dan 50 GB SSD.
c. Lugner 1GB, 1vCPU, dan 25 GB SSD.
aturlah agar Eisen dapat bekerja dengan maksimal, lalu lakukan testing dengan 1000 request dan 100 request/second. 

### Explanation
