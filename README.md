# book_algorithms
### Бинарный поиск (бинарный поиск по ответу)
#### формула
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
def checkproblemcount(days, params):
    n, k = params
    return (k + (k + days - 1)) * days // 2 >= n
```
