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
