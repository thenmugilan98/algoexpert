# algoexpert
def threenumsum(A, arr_size, sum): 
  
    result = []
    for i in range( 0, arr_size-2): 
  
        for j in range(i + 1, arr_size-1):  
       
            for k in range(j + 1, arr_size): 
                if A[i] + A[j] + A[k] == sum: 
                    result.append([A[i],A[j],A[k]])
                    
    if len(result)==0:
        return o;
    else:
        return result;
  
A = [1, 4, 45, 6, 10, 8,0,12] 
sum = 22
arr_size = len(A) 
result = threenumsum(A, arr_size, sum) 
if result == 0:
    print("no triplets found")
else:
    for i in result:
        print(i)
