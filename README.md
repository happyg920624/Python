# python 

#九九乘法表multiplication table multiplication
for i in range(1,10):
    print(i,end='')
    for j in range(1,10):
        print(format(i * j,"4d"),end='')
    print()

for i in range(1,10):
    for j in range(1,10):
        s=  i*j
        print ('%d * %d = %d ' %(i, j , s))
     print('\n')

for i in range(1,10):
    for j in range(1,10):
        s=  i*j
        print ('%d * %d = %d   ' %(i, j , s), end="")
     print('\n')

k=[1,2,3,4,5,6,7,8,9]
for i in k :
    for j in k:
        s=  i*j
        print ('%d * %d = %d   ' %(i, j , s), end="")
   print('\n')

i=1
while i < 10:
    j=1
    while j < 10:
        s=  i*j
        print ('%d * %d = %d ' %(i, j , s))
        j += 1
    i += 1
    print('\n')
    
#最大公因數GCD
num1 = int(input("請輸入第一個數字："))
num2 = int(input("請輸入第二個數字："))
m = max(num1, num2)
n = min(num1, num2)
r = m % n
while r != 0:
    m = n
    n = r
    r = m % n
print(num1, "和", num2, "的最大公因數為", n)
