# Project 3



## [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

**Örnek:** root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.



# Solution 3

**Step 1:**

    Root null olduğu için 7 root olarak atanır.
**Step 2:**

    5, root'tan küçük olduğu için root'un solunda bulunur.

**Step 3:**

    1, root'tan küçük olduğu için solunda yer alır. 5'in solundadır.

**Step 4:**

    8, root'tan büyük olduğu için root'un sağında yer alır.

**Step 5:**

    3, root'tan küçük olduğu için root'un solunda yer alır. 1'in sağındadır.

**Step 6:**

    6, root'tan küçük olduğu için root'un solunda yer alır. 5'in sağındadır.

**Step 7:**

    0, root'tan küçük olduğu için root'un solunda yer alır. 1'in solundadır.

**Step 8:**

    9, root'tan büyük olduğu için root'un sağında yer alır. 8'in sağındadır.

**Step 9:**

    4, root'tan küçük olduğu için root'un solunda yer alır. 3'ün sağındadır.

**Step 10:**

    2, root'tan küçük olduğu için root'un solunda yer alır. 3'ün solundadır.

Oluşan ağaç:

                            7
                         /     \
                      5           8
                   /    \            \
                 1        6            9
               /   \
              0      3
                  /     \
                2         4