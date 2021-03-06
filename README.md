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
 
## Contoh Sederhana
Saya paham Anda akan bertanya-tanya kenapa kita harus membuat direktori dengan nama seperti di atas dan apa hubungannya sama akun Github. Saya pun memiliki pertanyaan yang sama. Lalu saya melakukan eksperimen, dan hasil akhirnya saya temukan bahwa sebenarnya tidak perlu membuat direktori seperti di atas untuk tahap belajar. Berikut ini eksperimen saya:

1. Buat satu file bernama variabel.go tepat di bawah direktori G:\GoWorks\.
2. Isi dengan kode program berikut:
	```
	package main

	import "fmt"
	
	func main() {
		var nama string = "Amri Shodiq"
		var umur int = 18
		var beratbadan float64 = 55
	    fmt.Println(nama, umur, beratbadan)
	}
	```

3. Kemudian jalankan perintah berikut
	```
	D:\GoWorks>go run variabel.go
	```

4. Atau anda juga bisa langsung mencobanya secara online di tautan berikut: https://play.golang.org/ (atau klik tautan berikut jika anda malas untuk menyalin+tempel di halaman tersebut https://play.golang.org/p/6aQti0fQcO)
5. Perhatikan hasilnya! Anda sudah mencoba bagaimana mendeklarasikan variabel dan menampilkannya dengan Println.
Ini adalah contoh sangat sederhana bagaimana menulis program Go. 
5. Tapi dengan cara `go run ...` Anda tidak mendapatkan file executable. Lalu bagaimana mendapatkan file executable?
6. Cara pertama adalah dengan mengubah parameter `run` menjadi `build`, yaitu 
	``` 
	D:\GoWorks>go build variable.go
	```
7. Buat direktori variabel di bawah D:\GoWorks\, kemudian pindahkan file variabel.go ke dalam direktori D:\GoWorks\variabel\.
8. Sampai saat ini Anda memiliki file D:\GoWorks\variabel\variabel.go.
9. Compile dengan cara berikut:
	```
	D:\GoWorks>go install variabel
	```
10. Sampai tahap ini, Anda sudah dapat file D:\GoWorks\bin\variabel.exe.

