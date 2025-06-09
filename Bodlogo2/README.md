## Бодлогын нэр: Detect Cycle in a Linked List

🔗 **Холбоос**: [https://www.hackerrank.com/challenges/detect-whether-a-linked-list-contains-a-cycle?isFullScreen=true](https://www.hackerrank.com/challenges/detect-whether-a-linked-list-contains-a-cycle?isFullScreen=true)

---

Бодлогын Монгол орчуулга:

Танд `SinglyLinkedListNode` төрлийн холбоост жагсаалт өгөгдөнө. Энэхүү холбоост жагсаалт цикл (өөрөөр хэлбэл, зангилаа өөрийнхөө өмнөх эсвэл өмнөхийн өмнөх зангилаа руу зааж байгаа)
агуулж байгаа эсэхийг шалгана уу.

---

Шийдлийн тайлбар:

Энэхүү асуудлыг "Floyd's Cycle Detection Algorithm" буюу "Tortoise and Hare" аргыг ашиглан шийдэж болно:

1. Хоёр заагч (slow, fast) үүсгэнэ.
2. `slow` нь нэг алхам, `fast` нь хоёр алхмаар урагшилна.
3. Хэрвээ ямар нэгэн мөчид `slow == fast` болвол цикл байгаа гэсэн үг.
4. Хэрвээ `fast` эсвэл `fast.next` нь `null` болвол цикл байхгүй.

Цаг хугацааны төвөгшил: **O(n)**  
Санах ойн төвөгшил: **O(1)**

---

Жишээ:

**Input:**
```
1 → 2 → 3 → 4 → 2 (Циклтэй)
```

**Output:**
```
true
```

**Input:**
```
1 → 2 → 3 → 4 → null (Циклгүй)
```

**Output:**
```
false
```

