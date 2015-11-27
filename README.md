# Belajar Go Language

## Instalasi
1. Download dari [sini](https://storage.googleapis.com/golang/go1.5.1.windows-amd64.msi)
2. Jalankan file installer yang telah di download, kemudian pilih lokasi instalasi, saya sendiri lebih senang lokasi D:\Go\.
3. Installer akan secara otomatis menambahkan Environment Variable Path dengan D:\Go\bin.

## Test Hasil Instalasi
1. Buat direktori di mana nanti kita akan menaruh file-file kode program kita, atau workspace kita. Saya buat direktori baru D:\GoWorks\.
2. Tambahkan Environment Variable GOPATH dengan nilai D:\GoWorks.
3. Buat direktori D:\GoWorks\src\github.com\amrishodiq\hello. Ganti amrishodiq dengan username github Anda.
4. Kemudian tulis sebuah file bernama hello.go di dalam direktori tersebut. Isi file tersebut dengan baris-bari berikut:

```
package main

import "fmt"

func main() {
    fmt.Printf("Assalamu 'alaikum, Amri.\n")
}
```

5. Compile file baru Anda, hello.go, dengan perintah berikut

```
go install github.com/amrishodiq/hello
```
Tentu Anda harus mengganti amrishodiq dengan username Anda sendiri.

6. Kemudian, dengan DOS prompt, masuklah ke direktori D:\GoWorks. Cek di dalam direktori tersebut, jika semua lancar maka seharusnya ada direktori bin di dalam nya. Kemudian jalankan perintah ini (ketikkan teks setelah tanda > saja):

```
D:\GoWorks>.\bin\hello
```

7. Jika Anda mendapatkan tulisan 'Assalamu 'alaikum, Amri' maka buka halaman LinkedIn Anda, tambahkan skill baru: Go Programming!
8. Selamat, Anda bisa mengklaim diri Anda sebagai Go Programmer!
 

