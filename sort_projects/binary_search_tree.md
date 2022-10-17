# Binary Search Tree

## Proje 

[7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

## Çözüm

Yapı sağ ve sol alarak ayrılacak. Alınan referans veriye göre sağ tarafta veriden büyük, sol tarafta veriden küçük elemanlar bulunacak. 

Eğer dizinin ilk elemanını referans alacak olursak 7 "root" olur. Dizinin diğer elemanları root a kıyasla tree ye yerleştirilir. 


[7, "5", 1, 8, 3, 6, 0, 9, 4, 2] --> 5, 7'den küçük oluğu için 7'nin sol tarafına yerleştirilecek

[7, 5, "1", 8, 3, 6, 0, 9, 4, 2] --> 1, 7'den küçük ve 5'den küçük olduğu için 5'in sol tarafına yerleştirilecek.

[7, 5, 1, "8", 3, 6, 0, 9, 4, 2] --> 8, 7'den büyük olduğundan 7'nin sağ tarafına yerleştirilecek. 

[7, 5, 1, 8, "3", 6, 0, 9, 4, 2] -   --> Bu adımlarda yukarıdaki işlemlerin aynısı uygulanacak.
[7, 5, 1, 8, 3, 6, "0", 9, 4, 2]  |      
[7, 5, 1, 8, 3, 6, 0, "9", 4, 2]  |
[7, 5, 1, 8, 3, 6, 0, 9, "4", 2]  |
[7, 5, 1, 8, 3, 6, 0, 9, 4, "2"] -  

Eğer Binary Search Tree yapısı oluşturacak olursak aşağıdaki gibi bir yapı elde ederiz:


                    (7)         // 7 root olarak kabul edilirse 5, 1, 3, 6, 0, 4 ve 
                   /   \           2 7'den küçük olduğundan sol tarafa, 8 ve 9 7'den
                 (5)   (8)         büyük olduğundan sağ tarafa yerleştirilecek. 
                /   \     \       
              (1)   (6)   (9)      
             /   \
           (0)   (3)
                /   \
              (2)   (4)


