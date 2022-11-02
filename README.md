# JAM
Cara fix jam pada openwrt/linux jika anda tidak ada kuota/data utama.
# shell/bash script

```sh
wget -O /usr/bin/jam https://raw.githubusercontent.com/malikshi/jam/main/jam.sh && chmod +x /usr/bin/jam
```
# Edit script

```sh
nano /usr/bin/jam
```

Silahkan rubah `api.myxl.xlaxiata.co.id` dengan bug/websites yang dapat anda akses dengan gratis.

# Jalankan Command

Silahkan jalankan command berikut pada terminal.

```sh
jam
```

refresh openwrt dashboard dan cek apakah jam sudah singkron

# SETTING CRON

## Silahkan edit cron/cronjob/schedule pada OpenWRT

```sh
@reboot root /usr/bin/jam
```

## Linux Base

```sh
crontab -e
```
Copy & Paste

```sh
@reboot root /usr/bin/jam
```

Save


# Credits

- https://github.com/syisahi12/time_sync