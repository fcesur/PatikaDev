
# Problem 1.1:


## [22,27,16,2,18,6] -> Insertion Sort


Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

Big-O gösterimini yazınız.

Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız

Average case: Aradığımız sayının ortada olması
Worst case: Aradığımız sayının sonda olması
Best case: Aradığımız sayının dizinin en başında olması.


# Solution 1.1:


**Step 1:** [22,27,16,2,18,6] --> [22,27,16,2,18,6]

    22 < 27 olduğundan sıra değişmez.

**Step 2:** [22,27,16,2,18,6] --> [16,22,27,2,18,6]

    27 > 16 : true
    22 > 16 : true

    16 sayısı 22'nin soluna yerleşir.

**Step 3:** [16,22,27,2,18,6] --> [2,16,22,27,18,6]

    27 > 2 : true
    22 > 2 : true
    16 > 2 : true

    2 sayısı 16'nın soluna yerleşir.

**Step 4:** [2,16,22,27,18,6] --> [2,16,18,22,27,6]

    27 > 18 : true
    22 > 18 : true
    16 > 18 : false

    18 sayısı 22'nin soluna yerleşir.

**Step 5:** [2,16,18,22,27,6] --> [2,6,16,18,22,27]

    27 > 6 : true
    22 > 6 : true
    18 > 6 : true
    16 > 6 : true
    2 > 6 : false

    6 sayısı 16'nın soluna yerleşir.

**Time Complexity:**

- Worst Case : O(x<sup>2</sup>)

- Best Case : O(n)

- Average Case : O(x<sup>2</sup>)

        18 -> Average Case 

---

# Problem 1.2:

## [7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.



# Solution 1.2

**Step1:** [7,3,5,8,2,9,4,15,6] -> [2,3,5,8,7,9,4,15,6]

    default min: 7
    3 < 7 : true
    min : 3
    5 < 3 : false
    8 < 3 : false
    2 < 3 : TRUE
    min : 2
    9 < 2 : false
    4 < 2 : false
    15 < 2 : false
    6 < 2 : false
    
    2 sayısı, default minimum sayı 7 ile yer değiştirir.

**Step 2:** [2,3,5,8,7,9,4,15,6] -> [2,3,5,8,7,9,4,15,6]

    default min : 3
    5 < 3 : false
    8 < 3 : false
    7 < 3 : false
    9 < 3 : false
    4 < 3 : false
    15 < 3 : false
    6 < 3 : false

    3 sayısı ikinci minimum olarak pozisyonunu korur.

**Step 3:** [2,3,5,8,7,9,4,15,6] -> [2,3,4,8,7,9,5,15,6]

    default min : 5
    8 < 5 : false
    7 < 5 : false
    9 < 5 : false
    4 < 5 : TRUE
    min : 4
    15 < 4 : false
    6 < 4 : false

    4 sayısı, default minimum sayı 5 ile yer değiştirir.

**Step 4:** [2,3,4,8,7,9,5,15,6] -> [2,3,4,5,7,9,8,15,6]

    default min : 8
    7 < 8 : TRUE
    min : 7
    9 < 7 : false
    5 < 7 : TRUE
    min : 5
    15 < 5 : false
    6 < 5 : false

    5 sayısı, default minimum sayı 8 ile yer değiştirir.












