# TIL
Today I learned

## nevin, shig's solution
'''python
def is_prime(num):
    return num > 1 and not any(num % n == 0 for n in range(2,num))
'''
> This is simple, although it is going to be slow. 
