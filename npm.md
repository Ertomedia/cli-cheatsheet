# npm

## Perintah Umum

### Buat app baru

#### Nodejs

```bash
npx gitignore node
npm init -y
```

#### Nextjs

```bash
npm init next-app <project_name>
```

### Install dependencies

Jalankan perintah berikut dalam folder app yang sedang aktif.

```bash
npm i <package_name>
```

### Cek outdated package

**Outdated global**

```bash
npm outdated -g
```

**Outdated local**

```bash
npm outdated
```

### Update package

**Update global**

```bash
npm update -g <package_name>
```

**Update local**

```bash
npm update <package_name>
```

### Build package

Jalankan perintah berikut dalam folder project.

```bash
npm run build
```

### Semantic Versioning

```bash
npm version major
```

```bash
npm version minor
```

```bash
npm version patch
```

### Publish npm packages

```bash
npm login
npm publish
```

## Troubleshooting

### Cara mudah update `npm` di Windows lewat PowerShell

1. Buka PowerShell dengan opsi **Run as Administrator**
2. Ketik `Set-ExecutionPolicy Unrestricted -Scope CurrentUser -Force`
3. Install package `npm-windows-upgrade` dengan command,

   ```text
   npm install --global --production npm-windows-upgrade
   npm-windows-upgrade
   ```

4. Jika ingin langsung mengupgrade, jalankan perintah ini.

   ```text
   npm-windows-upgrade --npm-version latest
   ```

Referensi:

{% embed url="https://github.com/felixrieseberg/npm-windows-upgrade" %}



