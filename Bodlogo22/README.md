# Encryption
## Холбоос  
[Hackerrank - Encryption](https://www.hackerrank.com/challenges/encryption/problem)


## Тодорхойлолт
Өгөгдсөн нэг мөр string-ийг encryption аргаар шифрлэнэ.  
Encryption нь дараах алхамуудаас бүрдэнэ:

1. Өгөгдсөн string-ийн бүх зай (space) үсгийг хасна.
2. Үсгийн уртыг L гэж авна.
3. rows = floor(sqrt(L)), cols = ceil(sqrt(L)) гэж тооцно.
4. Хэрэв rows * cols < L бол rows-г 1-ээр нэмнэ.
5. Үсгүүдийг rows x cols хэмжээтэй хүснэгтэнд байрлуулна.
6. Хүснэгтийн багануудаар уншиж, үсгүүдийг нэг мөр болгон холбоно.

Жишээ:  
"haveaniceday" -> "hae and via ecy"


## Шийдлийн тайлбар  
- Зайгаа авч, уртыг тооцно.  
- Хүснэгт үүсгэж, багануудаар унших замаар шинэ үг үүсгэнэ.  
- Энэ нь шифрлэх арга юм.


