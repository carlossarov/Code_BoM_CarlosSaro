# Code_BoM_CarlosSaro
n=int(input("Type an integrer number (n>=0): "))

sumd=0

while n<0:
    n=int(input("Type an integrer numer (n>=0): "))

for i in range(1,n):
    if n%i == 0:
        sumd=sumd+i


if sumd<n:
    if sumd==1 and n!=1:
        print("Number %d is defective and prime" % (n))

    else:
        print("Number %d is defective" % (n))
        
elif sumd>n:
    print("Number %d is abundant" % (n))

else:
    print("Number %d is perfect" % (n))
