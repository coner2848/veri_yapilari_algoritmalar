# Insertion Sort
[Patika.dev](https://app.patika.dev)
## Proje Adımları

[22,27,16,2,18,6] -> Insertion Sort 

1. Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.
2. Big-O gösterimini yazınız.
3. Time Complexity: Average case: Aradığımız sayının ortada olması,Worst case: Aradığımız sayının sonda olması, Best case: Aradığımız sayının dizinin en başında olması.
4. Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.
5. [7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.

## Çözümler
### 1. Adım

[22,27,16,2,18,6] En küçük elemanı bulur ve dizinin ilk elemanının konumuna ekler. Orada bulunan elemanı ise en küçük sayının bulunduğu konuma ekler. Diğer elemanlarıda bu şekilde sıralar.
* [22,27,16,2,18,6] --> [22,27,16,"2",18,6] --> [2|,27,16,"22",18,6] _(en küçük elemanı buldu ve dizinin başına eklendi. dizinin başındaki eleman ile yerleri değiştirildi)_ 
* [2|,27,16,22,18,"6"] --> [2|,"6",16,22,18,"27"] --> [2,6|,16,22,18,27] _(aynı işlem bir önceki adımdaki gibi tekrar edecek)_
* [2,6|,"16",22,18,27] --> [2,6,16|,22,18,27]
* [2,6,16|,22,"18",27] --> [2,6,16|,"18","22",27] --> [2,6,16,18|,22,27]
* [2,6,16,18|,"22",27] --> [2,6,16,18,22|,27]
* [2,6,16,18,22|,"27"] --> [2,6,16,18,22,27|] --> [2,6,16,18,22,27]
* Dizinin sıralanmış son hali yukaridaki adımlarda olduğu gibi [2,6,16,18,22,27] şeklindedir.


### 2. Adım

Big-O gösterimi
* Worst Case : O(n^2)
* Avarage Case : O(n^2)
* Best Case : O(n)

### 3. Adım

* Best Case : [2,6,16,18,22,27] _(Hiç yer değiştirme yapmadan sıralamayı bitireceği için en iyi durum sıralı bir dizinin olmasıdır)_
* Worst Case : [27,22,18,16,6,2] _(Her eleman için dizide en başa kadar karşılaştırma yapılacağından en kötü durum tersten sıralı bir dizi olmasıdır. )_

### 4. Adım

Dizi sıralandığında [2,6,16,18,22,27] şeklindedir. Sıralı dizide "18" sayısı ortada bulunduğundan Average Case kapsamına girer. 

### 5. Adım

[7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre sıralandığındaki ilk 4 adımı aşağıdaki gibidir:

* [7,3,5,8,"2",9,4,15,6] --> [2|,3,5,8,"7",9,4,15,6] --> [2|,3,5,8,7,9,4,15,6]
* [2|,"3",5,8,7,9,4,15,6] --> [2,3|,5,8,7,9,4,15,6]
* [2,3|,5,8,7,9,"4",15,6] --> [2,3|,"4",8,7,9,"5",15,6] --> [2,3,4|,8,7,9,5,15,6]
* [2,3,4|,8,7,9,"5",15,6] --> [2,3,4|,"5",7,9,"8",15,6] --> [2,3,4,5|,7,9,8,15,6]




