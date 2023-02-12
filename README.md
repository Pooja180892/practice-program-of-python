
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
print('factorial of no. is =',f)
=====================================================================================
Python Program for Find sum of odd factors of a number
num = int(input('enter the no. = '))
l = []
for i in range(1,num+1):
    if num % i == 0:
        if i % 2 != 0:
            l.append(i)
print('sum of odd factor is =', sum(l))
==========================================================================================
Python Program to Check if binary representation is a palindrome
num = int(input('enter the no = '))
binary = bin(num)
binary = binary[2:]
if binary == (binary[::-1]):
    print('palindrom')
else:print('not palindrom')
===================================================================================
 Python Program for Number of elements with odd factors in a given range
 for i in range(10,21):
    lst=[]
    for j in range(1,i+1):
        if i%j==0:
            lst.append(j)
    if ((len(lst))%2)!=0:
            print('Number of elements with odd factors of ',i,lst)
    ======================================================================================
    Python Program for Common Divisors of Two Numbers
    n1 = int(input('enter 1st no.= '))
n2 = int(input('enter 2nd no = '))
for i in range(1,(min(n1,n2)+1)):
    if n1 % i ==0 and  n2 % i==0:
        print('Common Divisors of Two Numbers',i)
======================================================================================

    
    
    
    Python Program to Check if binary representation is a palindrome
    num = int(input('enter the no = '))
binary = bin(num)
binary = binary[2:]
if binary == (binary[::-1]):
    print('palindrom')
else:print('not palindrom')
print('factorial of no. is =',f)
