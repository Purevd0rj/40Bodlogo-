from pathlib import Path

# README.md content for "Contacts" problem
readme_content = """
# Contacts

🔗 **Бодлогын холбоос**: [https://www.hackerrank.com/challenges/contacts?isFullScreen=true](https://www.hackerrank.com/challenges/contacts?isFullScreen=true)

---

## 🧾 Бодлогын Монгол орчуулга

Танд дараах 2 төрлийн команд ирнэ:

1. `add name` — нэр нэмэх
2. `find partial` — тухайн `partial` тэмдэгтээр эхэлдэг нэрийн тоог хэвлэх

---

## Оролт
n ← командын тоо
<command1>
<command2>

- `add name`: `name` нэрийг холбоо барих жагсаалтад нэмнэ.
- `find partial`: `partial` тэмдэгтээр эхэлдэг бүх нэрийн тоог шинэ мөрөнд хэвлэнэ.

---

## Гаралт

- `find` команд бүрт, тухайн нөхцөлд таарах нэрийн тоог шинэ мөрөнд хэвлэнэ.

---

## Жишээ

```text
Input:
4
add hack
add hackerrank
find hac
find hak

Output:
2
0
```
### Шийдлийн тайлбар
Энэхүү асуудалд Trie (Prefix Tree) ашиглах нь хамгийн оновчтой:

add: Тэмдэгт бүрээр цааш салбарлаж хадгална.

find: partial-ийн төгсгөлд хүрэх хүртэл явж, тэр цэгээс доош хэдэн нэр байгааг тоолдог.
