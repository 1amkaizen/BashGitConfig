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
