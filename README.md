# book_algorithms
### Формула бинарный поиск
```
def lbinsearch(l, r, check, checkparams):
    while l < r:
        m = (l + r) // 2
        if check(m, checkparams):
            r = m
        else:
            l = m + 1
    return l
```    

#### где check некая формула проверки, к примеру
```
def check(m, checkparams):
    return m*m >=  checkparams
```
