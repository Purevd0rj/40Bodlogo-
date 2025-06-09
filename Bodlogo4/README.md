## Бодлогын нэр: Swap Nodes [Algo]

🔗 **Холбоос**: [https://www.hackerrank.com/challenges/swap-nodes-algo?isFullScreen=true](https://www.hackerrank.com/challenges/swap-nodes-algo?isFullScreen=true)

---

### Бодлогын Монгол орчуулга:

Танд хоёртын модны бүтэц өгөгдөнө. Модны node бүр нь индексээр дугаарлагдсан байна. Модны `k`-н давтамжтайгаар бүх зангилааны гүн `k`-н үржвэртэй тэнцүү бол swap хийх хэрэгтэй.

Swap гэдэг нь тухайн node-ийн зүүн ба баруун child-ийг солих гэсэн үг. Модыг swap хийсний дараа in-order traversal хийж хэвлэнэ.

---

### Шийдлийн тайлбар:

1. **Модыг байгуулах:** Танд өгөгдсөн индексүүдийг ашиглан модыг үүсгэнэ.
2. **Swap хийх:** k, 2k, 3k,... гүнд хүрэх node-уудын зүүн ба баруун хүүхдүүдийг солино.
3. **Traversal:** Мод бүрд swap хийсний дараа in-order traversal хийж хэвлэнэ.

---

### Жишээ:

**Input:**

```
indexes = [
  [2, 3],
  [-1, -1],
  [-1, -1]
]
queries = [1]
```

**Output:**
```
3 1 2
```

