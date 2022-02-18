maximum=int(input("Please enter the maximum value: "))
total=0
for Number in range(1,maximum+1):
    count=0;
    for i in range(2,(Number//2+1)):
        if(Number%i==0):
          count=count+1
          break
    if(count==0 and Number !=1):
       # print("%d"%Number)
        total=total+Number
print("Sum of prime numbers from 1 to %d=%d"%(maximum,total))
