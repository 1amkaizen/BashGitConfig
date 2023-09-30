# BashGitConfig

Tools untuk otomatisasi konfigurasi Git khususnya di terminal.

### fungsi
- Konfigurasi git
- menghasilkan kunci SSH
- menguji koneksi ke GitHub


menghasilkan kunci SSH dan menguji koneksi ke GitHub. 

# Instalasi

```
git clone https://github.com/1amkaizen/BashGitConfig/
```

```
cd BashGitConfig
```

```
./bashgitconfig
```

Kemudian masukkan username dan email github kalian.

Salin kode rsa nya dengan perintah

```
cat /root/.ssh/id_rsa.pub
```
**output:** 
```ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQCmqfelq7QwGIonz3PhYlNs7Y2ZbcTrEwY8ug++RV7cj3YjNjub+CmCF1DHZbJZTZJ1T0DfFT4VXqXngesByDZn36N2XuUnY67LYuqB8ZuxotFJPzwV+MP6DhGVJ0oIPX1OyEzJKgIZzwzV0HDivfgaUFKixmoFz5P3lqT5pQNI2WdcV3aCGx3LYoPpQe9c+IGf3lZQmBfkTndGl+OGtikHSa2MkXZt1EaMPG8rBQIUwNmKVDWQvjSbR/+itOX4qaZXVYNADYTfYleOhd7EoHAC9ZsGyLbhsHGekZTTSftFk+9vp/4pqa9FbXgsU+gqM7UifZEDSanRm8aUWmrEQXowyrI7iKUfv6dMKlao8aymZYCg5S254ho0hOP0n+8sVuP7DQ6RcuI5RjvaDNWKSnk6hQ00haPMKpBDUEXg3uBt4k21EEw4pToHdZYnNBIju8vcqdiPL4IVxFBk+fsS3Q0Pci6E5kz4mNzvyE5H49CpyNprMr6Lme8mEo7gPpg9ScM= 1amkaiz3n@gmail.com```


Salin outputnya dan buka **pengaturan** github dan masuk ke **SSH**, tambah **key** baru dan pastekan koda rsa nya. 


### Cek koneksi ke GitHub 

```
ssh -T git@github.com
```

**jika berhasil:** Hi username! You've successfully authenticated, but Github does
not provide shell access.

# Cara Manual

```
git config --global user.name "Your name here"
```

```
git config --global user.email "your_email@example.com"
```

```
git config --global color.ui true
```

```
git config --global core.editor emacs
```

### Untuk menghasilkan SSH Key

```
ssh-keygen -t rsa -C "your_email@example.com"
```

### Cek koneksi ke GitHub 

```
ssh -T git@github.com
```
**jika berhasil:** Hi username! You've successfully authenticated, but Github does
not provide shell access.
