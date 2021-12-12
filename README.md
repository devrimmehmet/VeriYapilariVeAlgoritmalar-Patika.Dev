# Veri Yapıları Ve Algoritmalar - Patika.Dev 
## Patika.Dev Eğitimi Kapsamındaki Veri Yapıları ve Algoritmalar Ödevlerim
### Proje 1
[22,27,16,2,18,6] -> Insertion Sort

* **a)** Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.
* **b)** Big-O gösterimini yazınız.
* **c)** Time Complexity: Average case: Aradığımız sayının ortada olması,Worst case: Aradığımız sayının sonda olması, Best case: Aradığımız sayının dizinin en başında olması.
* **d)** Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.


* **e)** [7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.

---

**a)**

[22,27,16,2,18,6] => Dizinin içinde en küçük değeri buluruz bunu ilk sıraya çekeriz ve ilk sıradakinide en küçük değerin yerine koyarız.

[2,27,16,22,18,6] => Artık ilk değerimizi kontrol etmemize gerek yok, fakat aynı işlemi ikinci değer için yapacağız. İlk değer hariç diğer değerlere bakarız ve en küçük değeri 2.sıra ile yer değiştiririz.

[2,6,16,22,18,27] => ilk iki değer hariç aynı işlem yapılır. Fark ettikki 3.değerimiz zaten olması gereken yerde 4.ye geçeriz direk.

[2,6,16,18,22,27] => işlem adımlarımız tamamlandı. Diğer sıralarda zaten olması gerektiği yerde.


**b)**

Big-O gösterimimiz = **O(n²)** 'dir.

**c) ve d)**

Time Complexity:[22,27,16,2,18,6] =>[2,6,16,18,22,27] dizi sıralandıktan sonra farklı durumlara göre değerlerimiz.

Average Case: O(n²) => 16,18 ortaki değerimiz. 

Worst Case: O(n²) => 27 sondaki değere en son ulaşacağız.

Best Case: O(n) => 2 ilk değerimiz en mükemmel durumdur bizim için.

Dizi sıralandıktan sonra 18 değeri bizim için Average Case durumuna düşer.

**e)**

0= [7,3,5,8,2,9,4,15,6] 

1= [2,3,5,8,7,9,4,15,6]

2= [2,3,4,8,7,9,5,15,6]

3= [2,3,4,5,7,9,8,15,6]

4= [2,3,4,5,6,9,8,15,7]


### Proje2
[16,21,11,8,12,22] -> Merge Sort

**a)** Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.

**b)** Big-O gösterimini yazınız.

---

**a)**

1 : [16,21,11,8,12,22] diziyi ikiye böleriz.

2 : [16,21,11] - [8,12,22] diziyi ikiye böleriz.

3 : [16,21] - [11] - [8,12] - [22] diziyi ikiye böleriz.

4 : [16] - [21] - [11] - [8] - [12] - [22] her biri teke düştükten sonra sıralamalı bir şekilde birleştirme işlemine başlarız.

5 : [16,21] - [8,11] - [12,22] blokları sıralama yaparak birleştirmeye devam.

6 : [8,11,16,21] - [12,22]

7 : [8,11,12,16,21,22] 

**b)**

O(nlogn)
