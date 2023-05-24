
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
====================================================================================
Python Program to Check if a count of divisors is even or odd
n1 = int(input('enter no.= '))
lst=[]
for i in range(1,(n1+1)):
    if n1%i==0:
        lst.append(i)
if len(lst)%2==0:
    print('count of divisiors is even and count is', len(lst))
else:
    print('count of divisiors is odd and count is', len(lst))
========================================================================================
Python Program to Find the minimum sum of factors of a number
num = int(input('enter no.= '))
sum=0
i = 2
while(i < num):
    while(num % i == 0):
        sum += i
        num /= i
    i += 1
sum+= num
print(sum)
==================================================================================================
Python Program to find Difference between sums of odd and even digits
num = int(input('enter no = '))
even = 0
odd = 0
st_no = str(num)
for i in range(len(st_no)):
    if i % 2 == 0:
        even += int(st_no[i])
    else:odd += int(st_no[i])
difference = even - odd
print('Difference between sums of odd and even digits = ',difference)
========================================================================================================
