ANDIKA RIFQI ISTANTO (163210002)
IRFANI DIAH NUR SAFITRI (173210006)
NUR VITA RIA DHATUN (173210005)
INDAH TRIYANI (173210003)
ARUM MAWAR SARI (173210007)

Imperative Programming
Dalam ilmu komputer, imperative programming adalah paradigma pemrograman yang mempunyai karakteristik berupa status dan insruksi/perintah untuk mengubah status program. Status diwakili oleh variabel sedangkan instruksi diwakili oleh statemen. Dalam banyak cara yang sama suasana hati yang imperatif dalam bahasa-bahasa alamiah mengungkapkan perintah untuk mengambil tindakan, program-program penting menentukan urutan perintah untuk komputer untuk melakukan.
Ciri-ciri pemrograman imperatif yaitu :
- Adanya instruksi/command/perintah/kalimat-kalimat perintah contoh : GOTO 10
- Adanya status yang berubah contoh : dengan adanya perintah GOTO 10 maka status program akan loncat mengerjakan statemen yang ada di line number 10 Istilah ini digunakan dalam pemrograman deklaratif bertentangan, yang mengungkapkan apa yang perlu dilakukan, tanpa resep bagaimana melakukannya dalam hal urutan tindakan yang harus diambil. Pemrograman fungsional dan logis adalah contoh pendekatan yang lebih deklaratif.

```python
imperative programming
from abc import ABC, abstractmethod
class AbstractClassExample(ABC):
    
    @abstractmethod
    def do_something(self):
        print("Some implementation!")
        
class AnotherSubclass(AbstractClassExample):

    def do_something(self):
        super().do_something()
        print("The enrichment from AnotherSubclass")
        
x = AnotherSubclass()
x.do_something()

Procedural Programming
Procedural Programming ataupun Object Orienterd Programming (OOP) merupakan bentuk struktur data dari algoritma pemrograman. Object Oriented Programming (OOP) adalah suatu metode pemrograman yang berbasiskan pada objek, secara singkat pengertian dari OOP adalah koleksi objek yang saling berinteraksi dan saling memberikan informasi satu dengan yang lainnya. Pemrograman Terstruktur adalah suatu proses untuk mengimplementasikan urutan langkah untuk menyelesaikan suatu masalah dalam bentuk program.
Procedural programming itu berorientasi pada aksi, berbanding terbalik dengan OOP yang berorientasi terhadap objek.
Perbedaan mendasar antara OOP dan pemrograman terstruktur adalah dengan menggunakan OOP maka dalam melakukan pemecahan suatu masalah kita tidak melihat bagaimana cara menyelesaikan suatu masalah tersebut (terstruktur) tetapi objek-objek apa yang dapat melakukan pemecahan masalah tersebut. Sedangkan untuk pemrograman terstruktur,  menggunakan prosedur/tata cara yang teratur untuk mengoperasikan data struktur.
Kelebihan Prosedural
•   efektif digunakan untuk menyelesaikan masalah kecil
•   memperhatikan urutan langkah-langkah perintah secara sistematis, logis , dan tersusun berdasarkan algoritma yang sederhana
Kekurangan Prosedural
•   Tidak cocok untuk menyelesaikkan masalah yang rumit, karena nantinya akan kesulitan menemukan solusi permasalahan ketika terjadi eror.


procedural programming
class PersegiPanjang:
   def __init__(self, panjang, lebar, harga_unit=0):
      self.panjang = panjang
      self.lebar = lebar
      self.harga_unit = harga_unit
   def get_keliling(self):
       return 2 * (self.panjang + self.lebar)
   def get_luas(self):
       return self.panjang * self.lebar
   def hitung(self):
      luas = self.get_luas()
      return luas * self.harga_unit
# breadth = 120 cm, length = 160 cm, 1 cm^2 = Rs 2000
r = PersegiPanjang(160, 120, 2000)
print("Luas Persegi Panjang: %s cm^2" % (r.get_luas()))
print("Harga Unit Persegi Panjang: Rs. %s " %(r.hitung()))

output:
Luas Persegi Panjang: 19200 cm^2
Harga Unit Persegi Panjang: Rs. 38400000

#!/usr/bin/env python

Object Oriented Programming
Pengertian OOP
OOP (Object Oriented Programming) adalah suatu metode pemrograman yang berorientasi kepada objek. Tujuan dari OOP diciptakan adalah untuk mempermudah pengembangan program dengan cara mengikuti model yang telah ada di kehidupan sehari-hari. Jadi setiap bagian dari suatu permasalahan adalah objek, nah objek itu sendiri merupakan gabungan dari beberapa objek yang lebih kecil lagi. Saya ambil contoh Pesawat, Pesawat adalah sebuah objek. Pesawat itu sendiri terbentuk dari beberapa objek yang lebih kecil lagi seperti mesin, roda, baling-baling, kursi, dll. Pesawat sebagai objek yang terbentuk dari objek-objek yang lebih kecil saling berhubungan, berinteraksi, berkomunikasi dan saling mengirim pesan kepada objek-objek yang lainnya. Begitu juga dengan program, sebuah objek yang besar dibentuk dari beberapa objek yang lebih kecil, objek-objek itu saling berkomunikasi, dan saling berkirim pesan kepada objek yang lain.


class Mobil:

    def __init__(self):
        self.__memperbaharui()

    def sopir(self):
        print('sopir')

    def __memperbaharui(self):
        print('perbaharui')

redcar = Mobil()
redcar.sopir()
#redcar.__updateSoftware()  not accesible from object.

Output:
perbaharui
sopir

class Orang:
  def __init__(self, nDepan, nBelakang):
    self.namadepan = nDepan
    self.namabelakang = nBelakang

  def cetaknama(self):
    print(self.namadepan, self.namabelakang)

x = Orang("Fani", "Vita")
x.cetaknama()

Output :
('Fani', 'Vita')
```python