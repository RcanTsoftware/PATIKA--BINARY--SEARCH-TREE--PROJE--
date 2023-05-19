# Binary Search Tree Projesi

<b>Soru 1:</b> [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

Örnek: root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

---
<b>Cevap 1:</b> Bir elemanı root olarak seçiyoruz. Sonra dizinin solundaki elemandan sağındaki elemana kadar teker teker karşılaştırıyoruz.Sıralamada zaten var olan eleman tekrar sıralamaya dahil edilmez.


Dengeli bir dağılım için (genellikle ortadaki eleman seçlir) root (kök boğum) olarak 7 elemanını seçiyorum.

<b>Aşamalar:</b>

1. Dizinin solundan elemanları teker teker inceliyorum. 7 ile 5 i karşılaştıracağım. 5, 7'den küçük olduğu için sol alt tarafa yazılır.
    + ```
                  7
                 /
                5

2. Üçüncü rakamımız " 1 ". 1, 7'den ve 5'ten de küçük olduğu içib en alt sola yerleştirilir.
    + ```
                  7
                 /
                5
               /
              1

3. Dördüncü rakamımız " 8 ". 7'den büyük olduğu için sağ alt tarafa yerleştirilir.
    + ```
                  7
                 / \
                5   8
               /
              1

4. Beşinci rakamımız " 3 ". 7'den ve 5'den küçük ve 1'den büyük olduğu için sağ alt tarafa yerleştirilir.
    + ```
                  7
                 / \
                5   8
               /
              1
               \
                3

5. Altıncı rakamımız " 6 ". 7'den küçük ve 5'ten büyük olduğu için sağ alt tarafa yerleştirilir.
    + ```
                  7
                 / \
                5   8
               / \
              1   6
               \
                3

6. Yedinci rakamımız " 0 ". 7'den , 5'ten ve 1'den küçük olduğu için sol alt tarafa yerleştirilir.
    + ```
                  7
                 / \
                5   8
               / \
              1   6
             / \
            0   3

7. Sekizinci rakamımız " 9 ". 7'den ve 8'den büyük olduğu için sağ alt tarafa yerleştirilir.
    + ```
                  7
                 / \
                5   8
               / \   \
              1   6   9
             / \
            0   3

8. Dokuzuncu rakamımız " 4 ". 7'den ve 5'sen küçük olduğu için sol , 1'den ve 3'den büyük olduğu için sağ alt tarafa yerleştirilir.
    + ```
                  7
                 / \
                5   8
               / \   \
              1   6   9
             / \
            0   3
                 \
                  4

9. Onuncu rakamımız " 2 ". 7'den , 5'den küçük olduğu için sol 1'den büyük olduğu için sağ 3'ten küçük olduğu için sol alt tarafa yerleştirilir.
    + ```
                  7
                 / \
                5   8
               / \   \
              1   6   9
             / \
            0   3
               / \
              2   4 