# Menggunakan Microsoft SQL Server pada Visual Studio Code
1. Pastikan vscode sudah diinstall sebelumnya
2. Buka vscode lalu install extension "mssql" pastikan extension dirilis oleh microsoft
3. Tekan CTRL + SHIFT + P lalu search "Open User Settings (JSON)"
4. Tambahkan code berikut, sesuaikan dengan server dan user masing-masing:
   ```bash
       "mssql.connections": [
        {
            "trustServerCertificate": true,
            "authenticationType": "SqlLogin",
            "profileName": "ISI",
            "server": "ISI",
            "database": "",
            "user": "ISI",
            "password": "ISI",
            "savePassword": true,
        },
   ```
6. Cek apabila ada kesalahan penulisan (merah), kalau tidak ada tekan CTRL + S tutup file settings, tutup vscode, kemudian buka lagi
7. Akan muncul bagian menu SQL Server pada sidebar
