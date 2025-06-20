# Queue using Two Stacks

🔗 **Бодлогын холбоос**: [https://www.hackerrank.com/challenges/queue-using-two-stacks/problem](https://www.hackerrank.com/challenges/queue-using-two-stacks/problem)

---

## Бодлогын Монгол орчуулга

Та **FIFO** зарчмаар ажилладаг **queue** бүтцийг **хоёр stack ашиглан** хэрэгжүүлэх ёстой.

Гурван төрлийн асуулт өгөгдөнө:

- `1 x` → тоо `x`-г queue-д нэм.
- `2` → queue-с хамгийн эхний элементийг устга.
- `3` → queue-ийн хамгийн эхний элементийг хэвлэ.

---

## Оролт

- Эхний мөрөнд `q` — асуултын тоо.
- Дараагийн `q` мөр бүрт 1, 2, эсвэл 3 төрлийн асуулт өгөгдөнө.

---

## Гаралт

- Зөвхөн 3-р төрлийн асуулт бүрийн үед гарц дээр нэг мөрөнд queue-ийн хамгийн эхний элемент гарна.

---

## Жишээ

**Оролт:**
10
1 42
2
1 14
3
1 28
3
1 60
1 78
2
3

**Гаралт:**
14
14
60


---

## Шийдлийн тайлбар

Stack бол **LIFO** бүтэц. Харин Queue бол **FIFO**. Queue-ийг stack ашиглан эмуляц хийхийн тулд **хоёр stack ашиглана**:

- `stackNewest` — шинэ нэмсэн утгууд.
- `stackOldest` — унших/устгах үед ашиглах.

### Queue-ийн үйлдэл бүрийн зарчим:

- `enqueue(x)` → `stackNewest.push(x)`
- `dequeue()` → Хэрэв `stackOldest` хоосон байвал `stackNewest`-с бүх элементийг `pop` хийгээд `stackOldest`-д `push` хийнэ, дараа нь `stackOldest.pop()`
- `peek()` → `stackOldest` дээрээс уншина (шаардлагатай бол дээрхтэй ижилээр шилжүүлэлт хийнэ)
- Queue-ийн `enqueue` болон `dequeue` нь **амортизласан O(1)** хугацаатайгаар ажиллана.
- `stackOldest` рүү шилжүүлэлт зөвхөн `stackNewest`-д байгаа бүх элементийг шилжүүлэх шаардлагатай үед хийгддэг.
- Stack → push/pop дээр төвлөрдөг.
- Queue → peek нь хамгийн урд элементийг үзэх тул урвуу дарааллаар хадгалах шаардлагатай.
- `stackNewest` → нэмэх
- `stackOldest` → хасах, харах

---
