
Python Program for Find largest prime factor of a number
n=int(input('enter the no.:'))
lst=[]
for i in range(1,n+1):
    if n%i==0:
        count=0
        for j in range(1,i+1):
            if i%j==0:
                count=count+1
        if count==2:
            lst.append(i)
print(lst)
print('largest prime factor of',n,'is',max(lst))
==============================================================================
Python Program for Product of unique prime factors of a number
n=int(input('enter the no.:'))
lst=[]
for i in range(1,n+1):
    if n%i==0:
        count=0
        for j in range(1,i+1):
            if i%j==0:
                count=count+1
        if count==2:
            lst.append(i)
from functools import reduce
print('unique prime factor of', n ,'is',reduce(lambda x,y:x*y , lst))
=======================================================================================
.Python Program to find Factorial of Number
num = int(input('enter the no. = '))
f = 1
while num > 0:
    f = f * num
    num -= 1
    
    Python Program to Check if binary representation is a palindrome
    num = int(input('enter the no = '))
binary = bin(num)
binary = binary[2:]
if binary == (binary[::-1]):
    print('palindrom')
else:print('not palindrom')
print('factorial of no. is =',f)
