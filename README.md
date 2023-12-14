from math import sqrt
 
def Prime(number,itr):  
  if itr == 1:   
    return True
  if number % itr == 0:  
    return False
  if Prime(number,itr-1) == False:   
    return False
     
  return True
  
num = 13
 
itr = int(sqrt(num)+1)
 
print(Prime(num,itr))
