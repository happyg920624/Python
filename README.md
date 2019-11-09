# python
for i in range(1,10):
    print(i,end='')
    for j in range(1,10):
        print(format(i * j,"4d"),end='')
    print()
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

