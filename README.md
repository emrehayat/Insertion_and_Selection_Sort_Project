# Insertion ve Selection Sort Projesi

## Patika Dev - Veri Yapıları ve Algoritmalar - Proje 1

### Insertion Sort Projesi

[22, 27, 16, 2, 18, 6] -> Insertion Sort

Yukarıda verilen dizinin sort türüne göre aşamalarını yazınız.

Big-O gösterimini yazınız.

Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız.

Average case: Aradığımız sayının ortada olması. <br/>
Worst case: Aradığımız sayının sonda olması. <br/>
Best case: Aradığımız sayının dizinin en başında olması.

## Cevap

Dizi: [22, 27, 16, 2, 18, 6]

### Insertion Sort Aşamaları:
1. 22<27 doğrudur ve aynı durur: **[22, 27, 16, 2, 18, 6]**
2. 27>16 ve 22>16 yani 16 en sola gelir: **[16, 22, 27, 2, 18, 6]**
3. 27>2, 22>2 ve 16>2 yani 2 artık en soldadır: **[2, 16, 22, 27, 18, 6]**
4. 27>18 ve 22>18 yani 18 iki tane sola kayar: **[2, 16, 18, 22, 27, 6]**
5. 27>6, 22>6, 18>6 ve 16>6 yani 6 dört tane sola kayar: **[2, 6, 16, 18, 22, 27]**

Böylelikle sıralama tamamlanır.

### Big-O Gösterimi
Bu sıralama işleminin **Big-O** gösterimi, her adımda bir önceki elemanla karşılaştırarak en kötü durumda her elemanı tek tek kontrol etmesi gerektiği için **O(n^2)**'dir.

### Time Complexity
Dizi sıralandıktan sonra **18** sayısının durumu:
- **Average Case:** 18 sayısı dizinin ortasında bulunuyor, dolayısıyla average case kapsamına girer.

---

### Selection Sort Projesi

**[7,3,5,8,2,9,4,15,6]** dizisinin Selection Sort'a göre ilk 4 adımını yazınız.

## Cevap

Dizi: [7, 3, 5, 8, 2, 9, 4, 15, 6]

### Selection Sort İlk 4 Adım:
1. En küçük değeri bul (2), baştaki (7) ile değiştir: **[2, 3, 5, 8, 7, 9, 4, 15, 6]**
2. Sonraki en küçük değeri bul (3), 2. sıradaki (3) ile değiştir: **[2, 3, 5, 8, 7, 9, 4, 15, 6]** Yani değişmedi.
3. Üçüncü en küçük değeri bul (4), 3. sıradaki (5) ile değiştir: **[2, 3, 4, 8, 7, 9, 5, 15, 6]**
4. Dördüncü en küçük değeri bul (5), 4. sıradaki (8) ile değiştir: **[2, 3, 4, 5, 7, 9, 8, 15, 6]**
5. Beşinci en küçük değeri bul (6), 5. sıradaki (7) ile değiştir: **[2, 3, 4, 5, 6, 9, 8, 15, 7]** İkinci adımda değişiklik olmadığı için bu adımı da eklemek istedim.
