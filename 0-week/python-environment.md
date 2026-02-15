# Python Environment
Python (Virtual) Environment (selanjutnya disebut venv) adalah container terisolasi untuk menjalankan python dan library yang terdapat di dalamnya, dan tidak terikat dengan Python Global.
Dengan demikian, setiap project dapat memiliki library dan/atau versi library yang berbeda, tergantung kebutuhan masing-masing project. Hal ini memudahkan pada fase development dan testing apabila terdapat permasalahan dan error, tinggal hapus folder venv spesifik.

``` python
Python Global
├── venv data-analitik
│   ├── library: pandas
│   └── library: numpy
└── venv web-automation
    └── library: selenium
```
