def ypologismos(n, sum) :
     
    if (n == 0) :
        return (sum == 0)
 
    if (sum == 0) :
        return 1
 
    a = 0

    for i in range(0, 10) :
        if (sum-i >= 0) :
            a = a + ypologismos(n-1, sum-i)
 
    return a
     
     
def ypologismos2(n, sum) :
     
   
    a = 0
 

    for i in range(1, 10) :
        if (sum-i >= 0) :
            a = a + ypologismos(n-1, sum-i)
 
    return a
 
 
n = input("enter digits: ")
sum = input("enter sum: ")
n=int(n)
sum=int(sum)
print(ypologismos2(n, sum))