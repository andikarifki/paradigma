ANDIKA RIFQI ISTANTO (163210002) INDAH TRIYANI (173210003) NUR VITA RIA
DHATUN (173210005) IRFANI DIAH NUR SAFITRI (173210006) ARUM MAWAR SARI
(173210007)
```python
def dist2D( p ): return (p[0]**2 + p[1]**2)\*\*0.5

pts = [ (4.5, 3), (2.1,-1), (6.8,-3), (1.4, 2.9) ] print(max(
map(dist2D,pts) ))
```
penjelasan :menggambarkan konsep bahwa Python memperlakukan fungsi sebagai objek "kelas satu" dengan kata lain fungsi dapat digunakan seperti variabel dan data lainnya
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
```python
def dist2D( p ): return list(map( lambda x: x\*\*2, [ 1, 2, 3, 4 ] ))

pts = [ (4.5, 3), (2.1,-1), (6.8,-3), (1.4, 2.9) ] print(max(
map(dist2D,pts) ))
```
penjelasan : mengkuadratkan nilai daftar
----------------------------------------
```python
n = 100 sum( map( lambda x: x\*\*2, range(1,n+1)))
```
penjelasan : kita bisa menjumlahkan kotak dari 1 ke n
-----------------------------------------------------
```python
def dist2D( p ): return max( map( lambda p: (p[0]**2 + p[1]**2)\*\*0.5,
pts) )

pts = [ (4.5, 3), (2.1,-1), (6.8,-3), (1.4, 2.9) ] print(max(
map(dist2D,pts) ))
```
penjelasan : Kami juga dapat mengimplementasikan fungsi dist2D secara anonim
----------------------------------------------------------------------------
```python
def dist2D( p ): return max( map( lambda p: (p[0]**2 + p[1]**2)\*\*0.5,
pts) )

pts = [ (6,-1), (8,4), (7.5,-3), (4.4,12), (7,2) ] print(max(
map(dist2D,pts) ))
```
penjelasan :daftar berikut dari x, tipe koordinat titik y,akan menggunakan map (), fungsi lambda, dan maks () untuk menemukan maksimum koordinat x (koordinat ke-0) dalam daftar poin.
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
```python
def dist2D( p ): return list(filter( lambda x: x\>0, v)) v = [ 1, 9, -4,
-8, 10, -3 ] pts = [ (6,-1), (8,4), (7.5,-3), (4.4,12), (7,2) ]
print(max( map(dist2D,pts) ))
```
penjelasan : bagaimana cara menghilangkan semua nilai negatif dari daftar. Berdasarkan apa yang di ketahui sejauh ini, ini membutuhkan for for loop dengan append
-----------------------------------------------------------------------------------------------------------------------------------------------------------------
```python
def dist2D( p ): return sum(filter( lambda x: x\>0, v)) v = [ 1, 9, -4,
-8, 10, -3 ] pts = [ (6,-1), (8,4), (7.5,-3), (4.4,12), (7,2) ]
print(max( map(dist2D,pts) ))
```
penjelasan : Fungsi lambda harus menghasilkan nilai boolean dan jika nilai itu Benar item daftar disimpan; jika tidak dihilangkan.Hasil filter adalah objek iterator, sama seperti hasil map
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
```python
def dist2D( p ): return sum(filter( lambda x: x\>0, v)) v = [ 1, 9, -4,
-8, 10, -3 ] pts = [ (2,5), (12,3), (12,1), (6,5), (14, 10), (12, 10),\
 (8,12), (5,3) ] print(max( map(dist2D,pts) ))
```
penjelasan : pengurutan daftar poin (x, y) berdasarkan nilai y mereka terlebih dahulu dan nilai x untuk nilai terikat y, keduanya dalam urutan menurun.
-------------------------------------------------------------------------------------------------------------------------------------------------------
```python
def dist2D( p ): return sum(filter( lambda x: x\>0, v)) v = [ 1, 9, -4,
-8, 10, -3 ] pts = [(8, 12), (14, 10), (12, 10), (6, 5), (2, 5), (12,
3),\
 (5, 3), (12, 1)] print(max( map(dist2D,pts) ))
```
penjelasan : pengurutan daftar poin (x, y) berdasarkan nilai y mereka terlebih dahulu dan nilai x untuk nilai terikat y, keduanya dalam urutan menurun
------------------------------------------------------------------------------------------------------------------------------------------------------
```python
def dist2D( p ): return sorted( pts, reverse=True ) v = [ 1, 9, -4, -8,
10, -3 ] pts = [(8, 12), (14, 10), (12, 10), (6, 5), (2, 5), (12, 3),\
 (5, 3), (12, 1)] print(max( map(dist2D,pts) ))
```
penjelasan :memberikan pesan dengan nilai x dan kemudian oleh nilai y
---------------------------------------------------------------------
```python
def dist2D( p ): return sorted( pts, key = lambda p: p[1], reverse=True)
v = [ 1, 9, -4, -8, 10, -3 ] pts = [(8, 12), (14, 10), (12, 10), (6, 5),
(2, 5), (12, 3),\
 (5, 3), (12, 1)] print(max( map(dist2D,pts) ))
```
penjelasan :Langkah pertama adalah menyediakan fungsi kunci untuk diurutkan () untuk mengeluarkan informasi (nilai y dalam kasus ini) dari setiap tuple untuk digunakan sebagai dasar untuk menyortir
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
```python
def dist2D( p ): return sorted( pts, key = lambda p: (p[1], p[0]),
reverse=True) pts = [(8, 12), (14, 10), (12, 10), (6, 5), (2, 5), (12,
3),\
 (5, 3), (12, 1)] print(max( map(dist2D,pts) ))
```
penjelasan : dapat memperpanjang lambda kita untuk membalikkan tuple yang disediakan untuk disortir ()
------------------------------------------------------------------------------------------------------
```python
exercise : print (); a = 1; b = 10; for ganjil in range (a,b,1): if
ganjil % 2 == 1 : print (ganjil);
```
penjelasan :diatas adalah perintah untuk menghasilkan daftar semua
pasangan nilai integer positif ganjil kurang dari 10 di mana nilai
pertama kurang dari nilai kedua.
