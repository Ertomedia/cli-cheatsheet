# Git

## Perintah umum

 Untuk bantuan ketik `git help`.

### Membuat repo baru

Jalankan perintah berikut dalam folder project.

```bash
git init
git add .
git commit -am 'Initial commit'
```

### Menambahkan remote git url

Beberapa cara yang dapat digunakan adalah,

```bash
git remote add origin <GIT_REPO_URL>
```

```bash
git remote add github <GITHUB_REPO_URL>
```

```bash
git remote add gitlab <GITLAB_REPO_URL>
```

Gabungan ketiga cara diatas, dalam 1 baris.

```bash
git remote set-url --add origin <GITHUB_REPO_URL> && git remote set-url --add origin <GITLAB_REPO_URL>
```

Pada saat mau `git push` tinggal eksekusi satu perintah ini.

```bash
git push -u origin master
```

### Mengecek alamat remote git url

```bash
git remote show origin
```

### Push data ke remote git

```bash
git push -u origin master
```

```bash
git push -u github master
```

### Pull data dari remote git

```bash
git pull origin master
```

```bash
git pull origin master --allow-unrelated-histories
```

```bash
git pull github master
```

### Mengganti url remote repo

```bash
git remote set-url origin <GIT_REPO_BARU>
```

### Clone repo

```bash
git clone <GIT_REPO_URL>
```

### Buat branch baru

```bash
git checkout -b <NAMA_BRANCH>
```

### Pindah ke branch lain

```bash
git checkout <NAMA_BRANCH>
```

### Merge perubahan dari branch lain

```bash
git merge <NAMA_BRANCH>
```

