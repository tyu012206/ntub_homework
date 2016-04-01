# 作業 003

* 請寫一段 Ruby 程式，把 `[1, 3, 5, 7, 9]` 變成 `[2, 4, 6, 8, 10]`
```
a = [1,3,5,7,9]
p a.map {|i| i+1 }
```
* 請印出在 1 到 2000 中，可以被 4 整除，但不能 100 整除，但又要可以被 400 整除的數字。(潤年計算公式)
```
p (1..2000).to_a.select{|num| (num %400==0 or (num%4==0 and num % 100!=0))}
```
* 請印出在 1 到 100 中所有單數的總和。
```
p (1..100).to_a.select{|num| num.odd?}.inject{|sum,n| sum+n}
```
* 請試著解釋什麼是 Symbol。
```
Symbols 就如同一個識別符號。一個 symbol 就代表它是”誰”了，而不是代表它是”什麼”。
```