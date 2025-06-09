## Бодлогын нэр: Is This a Binary Search Tree?

🔗 **Холбоос**: [https://www.hackerrank.com/challenges/is-binary-search-tree?isFullScreen=true](https://www.hackerrank.com/challenges/is-binary-search-tree?isFullScreen=true)

---

###  Бодлогын Монгол орчуулга:

Танд хоёртын мод өгөгдөнө. Энэ мод Binary Search Tree (BST) мөн эсэхийг шалгах хэрэгтэй.

BST нь дараах шинж чанарыг хангах ёстой:
1. Зүүн дэд мод дахь бүх node-уудын утга нь root node-с бага байна.
2. Баруун дэд мод дахь бүх node-уудын утга нь root node-с их байна.
3. Зүүн ба баруун дэд мод нь мөн BST байна.

---

### Шийдлийн тайлбар:

BST эсэхийг шалгахын тулд:
- Модыг in-order traversal хийнэ.
- In-order дараалал өсөхөөр байгаа эсэхийг шалгана.
- Эсвэл root-оос доош бүх node-уудын утгыг хамгийн бага, хамгийн их боломжит утгатай харьцуулан шалгана.

---

### Жишээ:

**Input:** BST бүтэцтэй мод  
**Output:** `true`

**Input:** BST биш мод  
**Output:** `false`


