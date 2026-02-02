# 95.-number-of-notes
def no_notes(a):
    Q = [500, 200, 100, 50, 20, 10] 
    x = 0
    for i in range(len(Q)):
        q = Q[i]
        x += a // q       
        a = a % q       
    if a > 0:           
        x = -1
    return x
print(no_notes(500))   
print(no_notes(560))  
print(no_notes(555))
output:
1
3
-1
