## Бодлогын нэр: Tree: Huffman Decoding

🔗 **Холбоос**: [https://www.hackerrank.com/challenges/tree-huffman-decoding?isFullScreen=true](https://www.hackerrank.com/challenges/tree-huffman-decoding?isFullScreen=true)

---

### Бодлогын Монгол орчуулга:

Танд Huffman кодчлолын мод (`Node root`) болон `s` гэсэн 0,1-ээс тогтсон кодчилсон тэмдэгт мөр өгөгдөнө. Энэ тэмдэгт мөрийг Huffman мод ашиглан тайлан, эх хэлбэрт нь буцаах функц бичнэ үү.

---

### Шийдлийн тайлбар:

Huffman мод нь дараах зарчмаар ажилладаг:
- Зүүн салаа → `0`
- Баруун салаа → `1`
- Навч (`leaf`) node → тодорхой тэмдэгт хадгалсан байна

Алгоритмын логик:
1. Root node-оос эхлэн `s` тэмдэгт мөрийн 0 болон 1-үүдийг ашиглан салаа даган явна.
2. Навч node-д хүрэх бүрт тухайн тэмдэгтийг хэвлэнэ.
3. Дараагийн тэмдэгтийг тайлахын тулд дахин root node руу очно.

---

### ✅ Жишээ:

**Input (кодчилол):**
```
1001011
```

**Модны бүтэц:**  
Модны бүтэц нь `Node` class ашиглан өгөгдсөн бөгөөд root node, left, right болон data-г агуулна.

**Output (тайлсан үг):**
```
ABACA
```
