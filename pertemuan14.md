ANDIKA RIFQI ISTANTO (163210002)
IRFANI DIAH NUR SAFITRI (173210006)
NUR VITA RIA DHATUN (173210005)
INDAH TRIYANI (173210003)
ARUM MAWAR SARI (173210007)

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

(base) E:\python>python latihan.py
Luas Persegi Panjang: 19200 cm^2
Harga Unit Persegi Panjang: Rs. 38400000

#!/usr/bin/env python

Encapsulation

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

(base) E:\python>python latihan.py
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

(base) E:\python>python latihan.py
('Fani', 'Vita')
```python