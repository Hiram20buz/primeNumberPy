https://inventwithpython.com/hacking/chapter23.html

https://www.baeldung.com/cs/prime-number-algorithms

https://byjus.com/maths/prime-factorization/#:~:text=The%20simplest%20algorithm%20to%20find,it%20cannot%20be%20further%20factorized.


Create algorithm using string concatenation and factorization 

The prime factors of 789 are: 3 and 263.

A composite number is a positive integer greater than 1 that has more than two distinct positive divisors. 

If a number is composite, it can be factored into smaller integers other than 1 and itself. For a composite number, at least one of its prime factors will be less than or equal to the square root of the number.

To clarify:

1. If a number \( n \) is composite, it can be expressed as \( n = a \times b \), where both \( a \) and \( b \) are integers greater than 1 and less than or equal to the square root of \( n \).

2. If \( n \) is a composite number, it will have at least one prime factor \( p \) such that \( p \leq \sqrt{n} \).

This property is useful in identifying whether a number is prime or composite. If a number has no divisors other than 1 and itself after testing divisibility up to its square root, then it's a prime number. If it has divisors other than 1 and itself within that range, it's a composite number.

```
s = lambda x: str(x)
i = lambda x: int(x)

789 = i(p(x) + p(1)) * i(p(y) + p(9))
789 = i(p(x) + p(3)) * i(p(y) + p(3))
789 = i(p(x) + p(7)) * i(p(y) + p(7))


```
Also,Every prime number can be written in the form of 6n + 1 or 6n – 1.

https://tutorax.com/blogue/en/what-are-all-the-prime-numbers/#:~:text=Except%20for%202%20and%203,if%20it's%20prime%20or%20not.&text=We%20now%20know%20that%205,and%2013%20are%20prime%20numbers.
```

decimalNumber = [1,2,3,4,5,6,7,8,9]
(1,1) = 1
(1,2) = 2
(1,3) = 3
(1,4) = 4
(1,5) = 5
(1,6) = 6
(1,7) = 7
(1,8) = 8
(1,9) = 9 >

(2,2) = 4
(2,3) = 6
(2,4) = 8
(2,5) = 10
(2,6) = 12
(2,7) = 14
(2,8) = 16
(2,9) = 18

(3,3) = 9 >
(3,4) = 12
(3,5) = 15
(3,6) = 18
(3,7) = 21
(3,8) = 24
(3,9) = 27

(4,4) = 16
(4,5) = 20
(4,6) = 24
(4,7) = 28
(4,8) = 32
(4,9) = 36

(5,5) = 25
(5,6) = 30
(5,7) = 35
(5,8) = 40
(5,9) = 45

(6,6) = 36
(6,7) = 42
(6,8) = 48
(6,9) = 54

(7,7) = 49 >
(7,8) = 56
(7,9) = 63

(8,8) = 64
(8,9) = 72

(9,9) = 81


```
Way to generate 9 are {(1,9), (3,3), (7,7)} -> digitGenerators = [1,3,7,9]

## Idea
Find the x and y.
- Calculate  the primer number less than or equal to the square root of the number.
- When doing so, generate only numbers whose last digits contain the list digitGenerators to save computer power.
- Also, you can save more power knowing that Every prime number can be written in the form of 6n + 1 or 6n – 1.
- Except for 2 and 3, any prime number can be written as '6n + 1' or '6n – 1'. So, if you have a number that isn't 2 or 3, try to express it in the form of 6n + 1 or 6n – 1 to see if it's prime or not. We now know that 5, 7, 11, and 13 are prime numbers.

# Prime Factorization
https://byjus.com/maths/prime-factorization/#:~:text=The%20simplest%20algorithm%20to%20find,it%20cannot%20be%20further%20factorized.

The issue is that for large numbers you have find a way to save computer power,maybe my approach can save it.


