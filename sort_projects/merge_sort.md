# Merge Sort

[Patika.dev](https://app.patika.dev)

## Proje

[16,21,11,8,12,22] -> Merge Sort

1. Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
2. Big-O gösterimini yazınız.

## Cozum

1. Dizi ikiye bölünüp sağ ve sol kısımlar kendi içinde sıralanır. Sağ ve sol kısımlar son haline geldiğinde birleştirilir.

                [16,21,11,8,12,22]
                   /         \
            [16,21,11]     [8,12,22]
             /    |         |    \
          [16] [21,11]     [8] [12,22]
           /   /    |       |    |   \
        [16] [21] [11]     [8] [12] [22]
         |     \   /        |    \   /
        [16]  [11,21]      [8]  [12,22]
           \   /             \   /
         [11,16,21]         [8,12,22]
                 \           /
               [8,11,12,16,21,22]
               
 2. Best Case : O(n*logn)
 3. 
    Average Case : O(n*logn)
              
    Worst Case : O(n*logn)            
