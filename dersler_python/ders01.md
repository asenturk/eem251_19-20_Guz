

```python
a=4
b=6
```


```python
a+b
```




    10




```python
b-a
```




    2




```python
a*b
```




    24




```python
b/a
```




    1.5




```python
b//a
```




    1




```python
b%a
```




    2




```python
b**a
```




    1296




```python
c="bu bir yazı "
c
```




    'bu bir yazı '




```python
c*3
```




    'bu bir yazı bu bir yazı bu bir yazı '




```python
print(c*3)
```

    bu bir yazı bu bir yazı bu bir yazı 
    


```python
c="bu bir yazı\n"
```


```python
print(c*3)
```

    bu bir yazı
    bu bir yazı
    bu bir yazı
    
    

**print ve input fonksiyonları**


```python
a=input("birinci sayıyı giriniz: ")
b=input("ikinci sayıyı giriniz: ")
c=a+b
print("girilen sayıların toplamı: ",c)
```

    birinci sayıyı giriniz: 10
    ikinci sayıyı giriniz: 20
    girilen sayıların toplamı:  1020
    


```python
a=input("birinci sayıyı giriniz: ")
b=input("ikinci sayıyı giriniz: ")
c=int(a) + int(b)
print("girilen sayıların toplamı: ",c)
```

    birinci sayıyı giriniz: 10
    ikinci sayıyı giriniz: 20
    girilen sayıların toplamı:  30
    


```python
a=input("birinci sayıyı giriniz: ")
b=input("ikinci sayıyı giriniz: ")
c=int(a) + int(b)
print(a,"sayısı ile",b,"sayısının toplamı: ",c)
```

    birinci sayıyı giriniz: 10
    ikinci sayıyı giriniz: 20
    10 sayısı ile 20 sayısının toplamı:  30
    


```python
'buraya yazdığım bir ifade string\'dir'
```




    "buraya yazdığım bir ifade string'dir"




```python
print('buraya yazdığım bir ifade string\'dir')
```

    buraya yazdığım bir ifade string'dir
    


```python
print("buraya yazdığım bir ifade string'dir")
```

    buraya yazdığım bir ifade string'dir
    


```python
a=3
b=10
c=a+b
print("{} ile {} sayısının toplamı: {}".format(a,b,c))
```

    3 ile 10 sayısının toplamı: 13
    


```python
a=3
b=10
c=a+b
print("{1} ile {0} sayısının toplamı: {2}".format(a,b,c))
```

    10 ile 3 sayısının toplamı: 13
    

**if else elif yapısı**


```python
a=int(input("bir sayı giriniz: "))
if a>10:
    print("girilen sayı 10'dan buyuktur")
```

    bir sayı giriniz: 20
    girilen sayı 10'dan buyuktur
    


```python
a=int(input("bir sayı giriniz: "))
if a>10:
    print("girilen {} sayısı 10'dan buyuktur".format(a))
```

    bir sayı giriniz: 20
    girilen 20 sayısı 10'dan buyuktur
    


```python
a=int(input("bir sayı giriniz: "))
if a>10:
    print("girilen {} sayısı 10'dan buyuktur".format(a))
else:
    print("girilen {} sayısı 10'dan kucuktur veya eşittir".format(a))
```

    bir sayı giriniz: 10
    girilen 10 sayısı 10'dan kucuktur veya eşittir
    


```python
a=int(input("bir sayı giriniz: "))
if a>10:
    print("girilen {} sayısı 10'dan buyuktur".format(a))
elif a==10:
    print("girilen sayı 10'a eşittir.")
else:
    print("girilen {} sayısı 10'dan kucuktur ".format(a))
```

    bir sayı giriniz: 5
    girilen 5 sayısı 10'dan kucuktur 
    


```python

```


```python
a=int(input("bir sayı giriniz: "))
if a>10:
    print("girilen {} sayısı 10'dan buyuktur".format(a))
elif a<=10 and a>5:
    print("girilen {} sayısı 10'a eşit veya 10'dan küçük ve 5'ten büyüktür.".format(a))
elif a==5:
    print("girilen sayı 5'e eşit")
else:
    print("girilen {} sayısı 5'den kucuktur ".format(a))
```

    bir sayı giriniz: 7
    girilen 7 sayısı 10'a eşit veya 10'dan küçük ve 5'ten büyüktür.
    

**karsılaştırma operatörleri:**   
\>, >=, <, <=, ==, !=   
&& $\rightarrow$ and     
|| $\rightarrow$ or  
! $\rightarrow$ not  


```python
a=2
b=3
```


```python
a==b
```




    False




```python
a!=b
```




    True




```python
a>=b
```




    False




```python
a<=b
```




    True




```python
a==2 and b==3
```




    True




```python
a==2 and b==1
```




    False




```python
a==2 or b==1
```




    True




```python
a==1 or b==1
```




    False




```python
not (a==1 or b==1)
```




    True



**Döngüler**


```python
i=1
while i<=10:
    print(i)
    i = i+1
```

    1
    2
    3
    4
    5
    6
    7
    8
    9
    10
    


```python
i=1
while i<=10:
    print(i,end="-")
    i = i+1
```

    1-2-3-4-5-6-7-8-9-10-


```python
i=1
while i<10:
    print(i,end="-")
    i = i+1
print(i)
```

    1-2-3-4-5-6-7-8-9-10
    


```python
list(range(10))
```




    [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]




```python
list(range(10))
```




    [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]




```python
list(range(10,30,3))
```




    [10, 13, 16, 19, 22, 25, 28]




```python
list(range(100,45,-3))
```




    [100, 97, 94, 91, 88, 85, 82, 79, 76, 73, 70, 67, 64, 61, 58, 55, 52, 49, 46]




```python
for i in range(10):
    print(i)
```

    0
    1
    2
    3
    4
    5
    6
    7
    8
    9
    


```python
for i in range(1,11):
    print(i, end="-")
```

    1-2-3-4-5-6-7-8-9-10-


```python
for i in range(1,10):
    print(i, end="-")
print(i+1)
```

    1-2-3-4-5-6-7-8-9-10
    

3'ün, 5'in veya 7'nin katı olan sayılar


```python
for i in range(1,100):
    if i%3==0 or i%5==0 or i%7==0:
        print(i, end=" ")
```

    3 5 6 7 9 10 12 14 15 18 20 21 24 25 27 28 30 33 35 36 39 40 42 45 48 49 50 51 54 55 56 57 60 63 65 66 69 70 72 75 77 78 80 81 84 85 87 90 91 93 95 96 98 99 

sayının asal olup olmadığını bulma


```python
a=5
for i in range(2,a):
    if a%i==0:
        break
        
if i != a-1:
    print("{} sayısı asal değildir. {} sayısına bölünür".format(a,i))
else:
    print("{} sayısı asaldır.".format(a))
```

    5 sayısı asaldır.
    


```python
a=101
for i in range(2,(a//2)+1):
    if a%i==0:
        break
        
if i == (a//2):
    print("{} sayısı asaldır.".format(a))
else:
    print("{} sayısı asal değildir. {} sayısına bölünür".format(a,i))
    
```

    101 sayısı asaldır.
    
