# python_questions
Some python questions

# 1) perfect number (Number whose addition of divisors is = number)
"""n=int(input("Enter the number to be checked: "))
sum=0
for i in range(1,n):
    if n%i==0 :
        sum+=i
if sum== n:
    print("The number entered is perfect.")
else:
    print("The number is not perfect.")
    
    
# 2) Armstrong Number (123=1**3+2**3+3**3)
n=int(input("Enter the number to be checked: ")) 
a=str(n)
sum=0
b=len(a)
for i in a:
    c=int(i)
    sum+= c**b
if sum==n:
    print("The number entered is armstrong.")
else:
    print("The number entered is not armstrong.")
    
# 3) Factorial (factorial of 5 = 1*2*3*4*5)
a=1
n=int(input("Enter the number whose factorial is to be find.:"))  
for i in range(1,n+1):
    a*=i
print(a)

# 4) Fibonacci series

a=[0,1,1,2,3,5,8,13]
b=[0,1]
n=int(input("Enter the number of terms series should have"))
if n<=0:
    print("Invalid operator")
if n==1:
    print([0])
if n==2:
    print([0,1])
if n >2:
    for i in range(0,n-2):
        z=b[-1]+b[-2]
        b.append(z) 
    print(b)
    
"""
a= input("enter your string")
b=len(a)

for i in range(0,b-1):
    if a[i]==a[b-i]:
        a="true"
if a=="true":
    print("palindrome")
else:
    print("not palindrome")
