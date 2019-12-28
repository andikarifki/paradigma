1. ANDIKA RIFQI ISTANTO (163210002)
2. IRFANI DIAH NUR SAFITRI (173210006)
3. NUR VITA RIA DHATUN (173210005)
4. INDAH TRIYANI (173210003)
5. ARUM MAWAR SARI (173210007)

# FUNCTIONAL PROGRAMMING
Functional programming adalah paradigma pemrograman yang berkutat pada komputasi yang terjadi di dalam fungsi matematis dan menghindari terjadinya perubahan data. Yang dimaksud dengan fungsi matematis sendiri adalah sebuah hubungan antara input yang akan mengembalikan output.

**fungsi murni**
Manfaat menggunakan fungsi murni daripada fungsi tidak murni (non-murni) adalah pengurangan efek samping . Efek samping terjadi ketika ada perubahan yang dilakukan dalam operasi fungsi yang berada di luar cakupannya. Misalnya, mereka terjadi ketika kita mengubah keadaan suatu objek, melakukan operasi I / O, atau bahkan memanggil print(). Contoh :

```python
class LineCounter:
    def __init__(self, filename):
        self.file = open(filename, 'r')
        self.lines = []

        def read(self):
            self.lines = [line for line in self.file]

        def count(self):
            return len(self.lines)
```

**kekekalan**

Pernahkah ada bug di mana Anda bertanya-tanya bagaimana variabel yang Anda setel menjadi 25 menjadi None ? Jika variabel itu tidak dapat diubah, kesalahan akan terjadi ketika variabel sedang diubah, bukan di mana nilai yang sudah berubah mempengaruhi perangkat lunak - akar penyebab bug dapat ditemukan sebelumnya.

Python menawarkan beberapa tipe data yang tidak berubah, yang populer adalah Tuple . Mari kita kontraskan Tuple ke Daftar , yang bisa berubah-ubah: 
```python
mutable_collection = ['Tim', 10, [4, 5]]
immutable_collection = ('Tim', 10, [4, 5])

# Reading from data types are essentially the same:
print(mutable_collection[2])    # [4, 5]
print(immutable_collection[2])  # [4, 5]

# Let's change the 2nd value from 10 to 15
mutable_collection[1] = 15

# This fails with the tuple
immutable_collection[1] = 15
```
**Fungsi Order Tinggi**
Dalam Python, fungsi diperlakukan sebagai objek kelas satu, memungkinkan Anda untuk melakukan operasi berikut pada fungsi.

-    Suatu fungsi dapat mengambil satu atau lebih fungsi sebagai argumen
-    Suatu fungsi dapat dikembalikan sebagai hasil dari fungsi lain 

Berfungsi sebagai argumen

Anda bisa meneruskan fungsi sebagai salah satu argumen ke fungsi lain. Ini ditunjukkan dalam contoh berikut. 

```python
def summation(nums): # normal function
    return sum(nums)

def main(f, *args): # function as an argument
    result = f(*args)
    print(result)

if __name__ == "__main__":
    main(summation, [1,2,3]) # output 6
 ```

**ekspresi lambda**
n ekspresi lambda untuk menulis fungsi Python. Sintaks lambda mengikuti sintaks def , tapi ini bukan pemetaan 1-ke-1. Berikut adalah contoh membangun fungsi yang menambahkan dua bilangan bulat:

```python
# Using `def` (old way).
def old_add(a, b):
    return a + b

# Using `lambda` (new way).
new_add = lambda a, b: a + bold_add(10, 5) == new_add(10, 5)
>> True
```
