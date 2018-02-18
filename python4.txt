lat = [(1000, 'M'),(900, 'CM'),(500, 'D'),(400, 'CD'),(100, 'C'),(90, 'XC'),(50, 'L'),
(40, 'XL'),(10, 'X'),(9, 'IX'),(5, 'V'),(4, 'IV'),(1, 'I')]

def metatropi(num):
	latin  = ''
	while num>0:
		for i,r in lat:
			while num >=i:
				latin += r
				num -=i
	return latin
num1 = input("enter number: ")
num1 = int(num1)
print(metatropi(num1))