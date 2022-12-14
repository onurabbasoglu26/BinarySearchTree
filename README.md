# Binary Search Tree Projesi
Patika.dev platformundaki "Veri Yapıları ve Algoritmalar" dersi Proje-3

***Ödev Sayfası:*** https://app.patika.dev/courses/veri-yapilari-ve-algoritmalar/binary-search-tree-proje

***Patika Profilim:*** https://app.patika.dev/ramones

# Soru ve Cevap
* [7,5,1,8,3,6,0,9,4,2] dizisinin Binary-Search-Tree aşamalarını yazınız.

**1.Adım:** Dizinin başlangıcı 7 olduğu için root 7'dir ve ağacın başına yazılır.

|Root=7|   |   |   |
|---|---|---|---|
|   |   |**7**|   |

**2.Adım:** 5 sayısı 7 den küçük olduğu için sola yazılır.

|5 Eklendi|   |   |   |
|---|---|---|---|
|   |   |   |**7**|
|   |   |***/***|   |
|   |**5**|   |   |

**3.Adım:** 1 sayısı 7'den ve 5'ten küçük olduğu için sola yazılır.

|1 Eklendi|   |   |   |   |   |
|---|---|---|---|---|---|
|   |   |   |   |   |**7**|
|   |   |   |   |***/***|   |
|   |   |   |**5**|   |   |
|   |   |***/***|   |   |   |
|   |**1**|   |   |   |   |

**4.Adım:** 8 sayısı 7'den büyük olduğu için 7'nin sağına yazılır.

|8 Eklendi|   |   |   |   |   |   |   |
|---|---|---|---|---|---|---|---|
|   |   |   |   |   |**7**|   |   |
|   |   |   |   |***/***|   |**\\**|   |
|   |   |   |**5**|   |   |   |**8**|
|   |   |***/***|   |   |   |   |   |
|   |**1**|   |   |   |   |   |   |

**5.Adım:** 3 sayısı 7'den küçük 5'ten küçük ve 1'den büyük olduğu için 1'in sağına yazılır.

|3 Eklendi|   |   |   |   |   |   |   |
|---|---|---|---|---|---|---|---|
|   |   |   |   |   |**7**|   |   |
|   |   |   |   |***/***|   |**\\**|   |
|   |   |   |**5**|   |   |   |**8**|
|   |   |***/***|   |   |   |   |   |
|   |**1**|   |   |   |   |   |   |
|   |   |**\\**|   |   |   |   |   |
|   |   |   |**3**|   |   |   |   |

**6.Adım:** 6 sayısı 7'den küçük 5'ten büyük olduğu için 5'in sağına yazılır.

|6 Eklendi|   |   |   |   |   |   |   |
|---|---|---|---|---|---|---|---|
|   |   |   |   |   |**7**|   |   |
|   |   |   |   |***/***|   |**\\**|   |
|   |   |   |**5**|   |   |   |**8**|
|   |   |***/***|   |**\\**|   |   |   |
|   |**1**|   |   |   |**6**|   |   |
|   |   |**\\**|   |   |   |   |   |
|   |   |   |**3**|   |   |   |   |

**7.Adım:** 0 sayısı 7'den küçük 5'ten küçük ve 1'den de küçük olduğu için 1'in soluna yazılır.

|0 Eklendi|   |   |   |   |   |   |   |   |   |
|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   |**7**|   |   |
|   |   |   |   |   |   |***/***|   |**\\**|   |
|   |   |   |   |   |**5**|   |   |   |**8**|
|   |   |   |   |***/***|   |**\\**|   |   |   |
|   |   |   |**1**|   |   |   |**6**|   |   |
|   |   |***/***|  |**\\**|   |   |   |   |   |
|   |**0**|   |   |   |**3**|   |   |   |   |

**8.Adım:** 9 sayısı 7'den büyük ve 8'den de büyük olduğu için 8'in sağına yazılır.

|9 Eklendi|   |   |   |   |   |   |   |   |   |   |   |
|---|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   |**7**|   |   |   |   |
|   |   |   |   |   |   |***/***|   |**\\**|   |   |   |
|   |   |   |   |   |**5**|   |   |   |**8**|   |   |
|   |   |   |   |***/***|   |**\\**|   |   |   |**\\**|   |
|   |   |   |**1**|   |   |   |**6**|   |   |   |**9**|
|   |   |***/***|  |**\\**|   |   |   |   |   |   |   |
|   |**0**|   |   |   |**3**|   |   |   |   |   |   |

**9.Adım:** 4 sayısı 7'den küçük 5'ten küçük 1'den büyük ve 3'ten büyük olduğu için 3'ün sağına yazılır.

|4 Eklendi|   |   |   |   |   |   |   |   |   |   |   |
|---|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   |**7**|   |   |   |   |
|   |   |   |   |   |   |***/***|   |**\\**|   |   |   |
|   |   |   |   |   |**5**|   |   |   |**8**|   |   |
|   |   |   |   |***/***|   |**\\**|   |   |   |**\\**|   |
|   |   |   |**1**|   |   |   |**6**|   |   |   |**9**|
|   |   |***/***|  |**\\**|   |   |   |   |   |   |   |
|   |**0**|   |   |   |**3**|   |   |   |   |   |   |
|   |   |   |   |   |   |**\\**|   |   |   |   |   |
|   |   |   |   |   |   |   |**4**|   |   |   |   |

**10.Adım:** 2 sayısı 7'den küçük 5'ten küçük 1'den büyük ve 3'ten küçük olduğu için 3 ün soluna yazılır.

|2 Eklendi|   |   |   |   |   |   |   |   |   |   |   |
|---|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   |**7**|   |   |   |   |
|   |   |   |   |   |   |***/***|   |**\\**|   |   |   |
|   |   |   |   |   |**5**|   |   |   |**8**|   |   |
|   |   |   |   |***/***|   |**\\**|   |   |   |**\\**|   |
|   |   |   |**1**|   |   |   |**6**|   |   |   |**9**|
|   |   |***/***|  |**\\**|   |   |   |   |   |   |   |
|   |**0**|   |   |   |**3**|   |   |   |   |   |   |
|   |   |   |   |***/***|   |**\\**|   |   |   |   |   |
|   |   |   |**2**|   |   |   |**4**|   |   |   |   |