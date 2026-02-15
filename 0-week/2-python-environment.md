# Python Environment
Python (Virtual) Environment (selanjutnya disebut venv) adalah container terisolasi untuk menjalankan python dan library yang terdapat di dalamnya, dan tidak terikat dengan Python Global.
Dengan demikian, setiap project dapat memiliki library dan/atau versi library yang berbeda, tergantung kebutuhan masing-masing project. Hal ini memudahkan pada fase development dan testing apabila terdapat permasalahan dan error, tinggal hapus folder venv spesifik tanpa harus merusak dan/atau melakukan install ulang Python Global.

Breakdown Python dan venv serta library masing-masing:

``` python
Python Global
├── venv data-analitik
│   ├── library: pandas
│   └── library: numpy
└── venv web-automation
    └── library: selenium
```

---

## Membuat Venv
Proses pembuatan venv melalui terminal atau powershell:
1. Buka terminal atau powershell
2. Pada contoh ini akan di buat pada drive D: -- maka langkah awal kita akan masuk ke drive D: melalui terminal
   ``` bash
   cd D:
   ```
3. Buat folder venv yang selanjutnya akan berisi semua venv
   ``` bash
   mkdir venv
   ```
4. Masuk ke dalam folder venv yang telah dibuat
   ``` bash
   cd venv
   ```
5. Buat venv, dalam contoh ini venv bernama "data" (jangan menggunakan nama yang panjang atau spasi)
   ``` python
   python -m venv data
   ```
6. Tunggu proses selesai, bisa dicek saat ini ini apakah pada drive D:/venv telah ada folder baru bernama "data" jika sudah maka venv berhasil dibuat.

---

## Menginstall library pada venv data
1. buka terminal dan masuk ke folder Scripts dalam venv
   ``` bash
   cd D:\venv\data\Scripts
   ```
2. Aktivasi venv dengan menjalankan
   ``` bash
    ./activate
   ```
   atau
   ``` bash
   ./Activate.ps1
   ```
3. Jika berhasil akan muncul nama venv pada baris awal command dalam hal ini akan muncul "(data)"
4. upgrade package package installer python terlebih dahulu
   ``` python
   python -m pip install --upgrade pip
   ```
5. Install library yang dibutuhkan, contoh kita akan menginstall pandas dan numpy
   ``` python
   pip install pandas numpy
   ```
6. Setelah selesai python environment dapat digunakan di vscode
7. Buka vscode buat file baru, pada pojok kanan bawah akan ada python dan versi python
8. Klik pada nomor versi >> "Enter interpreter path" >> Find.. Browse >> Buka folder venv/data/Scripts kemudian pilih python.exe
9. Apabila terdapat library yang kurang saat code dijalankan, ulangi proses aktivasi poin 2 dan install seperti poin 5, sesuaikan nama library.
