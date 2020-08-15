---
description: firebase adalah tool untuk deploy static site atau web app ke Firebase.
---

# Firebase

 Live demo: [https://climyid.web.app/](https://climyid.web.app/)

## Perintah Umum

 Untuk bantuan ketik `firebase help`.

### Deploy project ke hosting

```bash
firebase login
firebase init
firebase deploy
```

### Deploy multisite dalam project di hosting

1.  Di web console Firebase, pilih **Add another site** dan tentukan nama project-nya.
2.  Jalankan command `firebase login` dalam folder project.
3.  Setelah itu `firebase init` dan ikuti langkahnya.
4.  Edit file `firebase.json` dan tambahkan baris berikut,

   ```text
    .
        "hosting": {
            "site": "nama_project_di_hosting",
            .
        }
   ```

5. Simpan filenya, lalu jalankan command `firebase deploy --only hosting:namaproject`

