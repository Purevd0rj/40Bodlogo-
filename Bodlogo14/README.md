# Down to Zero II

🔗 **Бодлогын холбоос**: [https://www.hackerrank.com/challenges/down-to-zero-ii/problem](https://www.hackerrank.com/challenges/down-to-zero-ii/problem)

---

## 🧾 Бодлогын Монгол орчуулга

Танд бүхэл тоо `n` өгөгдсөн. Таны зорилго бол уг тоог **0** болгох явдал юм. Дараах хоёр үйлдлийн аль нэгийг ашиглан:

1. `n → n - 1`
2. Хэрэв `n` нь `a * b` хэлбэртэй бол `n → max(a, b)`

Хамгийн бага алхмаар 0 болгохын тулд хэдэн үйлдэл хийх шаардлагатай вэ?

---

## Оролт

t ← тестийн тоо
n₁
n₂
...
nₜ

---

## Гаралт

Тест бүрийн хувьд хамгийн бага хэдэн үйлдлээр 0 болгохыг хэвлэнэ.

---

## Жишээ

**Оролт:**
3
3
4
5


**Гаралт:**
3
3
4


---

## 🧠 Шийдлийн тайлбар

Энэ бол **графын хамгийн богино зам** (shortest path in an unweighted graph) олдог асуудал бөгөөд **BFS (Breadth First Search)** алгоритм ашиглана.

- Тухайн `n` тоог node гэж үзээд:
  - `n - 1` болон
  - `n → max(i, n/i)` (хэрэв `i * (n/i) == n`)
  
  гэсэн ирмүүд (edges) үүсгэнэ.
  
- BFS-ээр хамгийн түрүүнд 0-д хүрэх замын уртыг олно.
- BFS нь unweighted графын хувьд хамгийн богино замыг олдог батлагдсан арга.
- Хэрэглэж болох хязгаар (n ≤ 10⁶) тул **массив-based BFS** боломжийн гүйцэтгэлтэй.
- `n → n - 1` нь үргэлж боломжтой.
- Хоёр дахь үйлдлийг зөвхөн **үржвэрүүд байгаа тохиолдолд** хэрэглэх хэрэгтэй.

---



