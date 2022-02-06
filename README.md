# Insertion Sort Projesi

## Proje 1

`[22,27,16,2,18,6]` -> Insertion Sort

1. Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.
2. Big-O gösterimini yazınız.
3. Time Complexity:
   - Average case: Aradığımız sayının ortada olması,
   - Worst case: Aradığımız sayının sonda olması,
   - Best case: Aradığımız sayının dizinin en başında olması.
4. Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.
5. `[7,3,5,8,2,9,4,15,6]` dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.

---

## Sonuçlar

1. Dizinin aşamaları şu şekilde gerçekleşmiştir:

```
[2,27,16,22,18,6]
[2,6,16,22,18,27]
[2,6,16,18,22,27]
```

2. Big-O gösterimi şu şekildedir:

   $$
   [22,27,16,2,18,6] : n \newline
   [2,27,16,22,18,6] : n-1 \newline
   [2,6,16,22,18,27] : n-3 \newline
   [2,6,16,18,22,27] : 1 \newline
   $$

3. Binary Search Tree araması üzerinden:
   - Best & Average case: $O( \log n)$
   - Worst case: $O(n)$
4. Dizi sıralandıktan sonra, binary search tree aramasında best case kapsamına girer. (Dengeli dağılım varsayılmaktadır.)
5. İlk dört adım:

```
[2,3,5,8,7,9,4,15,6]
[2,3,4,8,7,9,5,15,6]
[2,3,4,5,7,9,8,15,6]
[2,3,4,5,6,9,8,15,7]
```

---

### Not:

Algoritma kontrolü için yazdığım kod vd. `insertionSort.html` dosyasındadır. Pekte bir şey yok pekiştirmek için sadece.

Birde burada kullanılan insertion sort algoritması aslında selection sort algoritmasıdır. Sadece eğitim icabı isim farklı geçmiştir.
