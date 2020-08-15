# PowerShell

## Perintah Umum

### Cek versi WSL distro Linux yang terinstall

```bash
wsl -l -v
```

### Ubah versi ke WSL 2 distro Linux yang terinstall

```bash
wsl --set-version <NAME> 2
```

### Run As Administrator

```bash
Start-Process Powershell -Verb runAs
```

### Update PowerShell

Jalankan PowerShell sebagai Administrator dulu.

```bash
iex "& { $(irm https://aka.ms/install-powershell.ps1) } -UseMSI"
```

### Empty Recycle Bin

```bash
Clear-RecycleBin -Force
```

