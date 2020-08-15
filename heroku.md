---
description: heroku adalah tool untuk deploy static site ke Heroku.
---

# Heroku

## Instalasi

 Dengan menggunakan `npm`

```bash
npm install -g heroku
```

 Untuk cara install alternatif bisa mengikuti langkahnya lewat [panduan ini](https://devcenter.heroku.com/articles/heroku-cli).

## Perintah umum

 Untuk bantuan ketik `heroku help`.

### Update program

```bash
heroku update
```

### Pre-deploy

Bagian ini adalah persiapan sebelum deploy ke Heroku. Jalankan command dalam folder project.

```bash
heroku login
```

Untuk project yang git repository-nya belum aktif, lakukan langkah berikut.

```bash
git init
heroku git:remote -a <NAMA_PROJECT>
```

Yang sudah aktif, gunakan langkah ini.

```bash
heroku git:remote -a <NAMA_PROJECT>
```

### Deploy/update ke Heroku

```bash
git add .
git commit -am "Initial commit"
git push heroku master
```

## Buildpacks yg tersedia

```text
heroku/nodejs
heroku/python
heroku/php
heroku/ruby
heroku/java
heroku/go
heroku/gradle
heroku/scala
heroku/clojure
```

