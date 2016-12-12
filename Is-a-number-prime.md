# Daily Codewars \#1
## Question
https://www.codewars.com/kata/is-a-number-prime/train/python
Define a function isPrime that takes one integer argument and returns true or false depending on if the integer is a prime. Per Wikipedia, a prime number (or a prime) is a natural number greater than 1 that has no positive divisors other than 1 and itself.

Example:
'''python
isPrime(5)
=>true
'''
You can assume you will be given an integer input.
You cannot assume that the integer will be only positive. You may be given negative numbers.

## My solution
'''python
def is_prime(num): 
    if num==2 or num==3:
        return True
    elif num>4:
        i=2
        while (num%i!=0 and i<(num+1)/2):
            i=i+1
        return i>num/2
    else:
        return False
'''
> Using if and while statements, I checked divisibility by 2 to n/2. 

## nevin, shig's solution
'''python
def is_prime(num):
    return num > 1 and not any(num % n == 0 for n in range(2,num))
'''
> This is simple, although it is going to be slow. 
