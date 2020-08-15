---
description: Chocolatey adalah package manager untuk Windows.
---

# Chocolatey

## Kebutuhan sistem

1. Windows 7+ / Windows Server 2003+
2. PowerShell v2+ \(minimum is v3 for install from this website due to [TLS 1.2 requirement](https://chocolatey.org/blog/remove-support-for-old-tls-versions)\)
3. .NET Framework 4+ \(the installation will attempt to install .NET 4.0 if you do not have it installed\)\(minimum is 4.5 for install from this website due to [TLS 1.2 requirement](https://chocolatey.org/blog/remove-support-for-old-tls-versions)\)

## Instalasi

1. Jalankan PowerShell dengan mode Administrator.
2. Eksekusi dalam PowerShell perintah `Set-ExecutionPolicy Bypass -Scope Process`
3. Setelah itu jalankan perintah berikut,

   ```text
   Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
   ```

4. Tunggu sampai selesai, jika tidak muncul pesan error jalankan `choco`.

## Perintah Umum

### Cek package yang butuh update

```text
choco outdated
```

### Update package

```text
choco upgrade <NAMA_PACKAGE> -y
```

```text
choco upgrade all -y
```

### Cek package yang terpasang

```text
choco list --local-only
```

### Cari package

```text
choco search <NAMA_PACKAGE>
```

### Install package

```text
choco install <NAMA_PACKAGE> <NAMA_PACKAGE> <NAMA_PACKAGE> -y
```

### Hapus package

```text
choco uninstall <NAMA_PACKAGE> -y
```

```text
choco uninstall all -y
```

