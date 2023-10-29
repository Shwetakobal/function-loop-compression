Q1. Which keyword is used to create a function? Create a function to return a list of odd numbers in the
range of 1 to 25.
def keyword is used to create a function
FUNCTION-USE INCREASE REUSABILITY,MODULARITY DATA
    def test2():
    return(1,3,5,7,9,11,13,15,17,19,21,23,25
    test2()
    (1, 3, 5, 7, 9, 11, 13, 15, 17, 19, 21, 23, 25)

Q2. Why *args and **kwargs is used in some functions? Create a function each for *args and **kwargs
to demonstrate their use.
ANS *args=*- you can pass n number of data ,allow pass multiple input, args= convention,argument
example
  def test1(*args):
    return args
    test1(1,2,3,4)
    (1, 2, 3, 4)
    
  def test12(*args,a):
    return args,a
    
   test12(1,2,3,4, a= 23)
   ((1, 2, 3, 4), 23)

**kwargs=keyword arguments pass dictionary type data like-key-value type of data is passing this is called *kwargs
example
   def test23(**kwargs):
       return kwargs
       
   test23(a="su", b="shweta")
        {'a': 'su', 'b': 'shweta'}
        
Q3. What is an iterator in python? Name the method used to initialise the iterator object and the method
used for iteration. Use these methods to print the first five elements of the given list [2, 4, 6, 8, 10, 12, 14,
16, 18, 20].
ans: In Python, an iterator is an object that allows you to iterate over collections of data, such as lists, tuples, dictionaries, and sets. Python iterators implement the iterator design pattern, which allows you to traverse a container and access its elements
 _init_() Name the method used to initialise the iterator object and the method used for iteration.
 l=[2, 4, 6, 8, 10, 12, 14,16,18,20]
 s1 = iter(l)
 next(s1)
 2
 next(s1)
 4
 next(s1)
 6
 next(s1)
 8
 next(s1)
 10
         
Q4. What is a generator function in python? Why yield keyword is used? Give an example of a generator
function.
ans: generator function is a special type of function.it generates outcome contiously without holding everything into a  memory.
     yield is special reveresed keyword it helps generate function
     def test_fib(n):
    a,b=0,1
    for i in range(n):
        yield a
        a,b=b,a+b
        
   for i in test_fib(12):
    print(i)
    0
    1
    1
    2
    3
    5
    8
    13
    21
    34
    55
    
Q5. Create a generator function for prime numbers less than 1000. Use the next() method to print the
first 20 prime numbers. 
ans: The prime numbers from 1 to 1000 can be listed if we find out the number of factors of each number. We know that a prime number is a number with only two factors, 1 and the number itself. For example, let us take the number 11 which has only two factors which are 1 and 11 itself. So, 11 is a prime number.

Q6. Write a python program to print the first 10 Fibonacci numbers using a while loop.
ans  def test_fib1():
      a,b=0,1
      while True:
        yield a
        a,b= b, a+b
        
   fib = test_fib1()
   
   for i in range(10):
    print(next(fib))
    0
    1
    1
    2
    3
    5
    8
    13
    21
    34
                
Q7. Write a List Comprehension to iterate through the given string: ‘pwskills’.
Expected output: ['p', 'w', 's', 'k', 'i', 'l', 'l', 's']
ans: l=[letter for letter in 'pwskills']
print(l)
['p', 'w', 's', 'k', 'i', 'l', 'l', 's']

Q8. Write a python program to check whether a given number is Palindrome or not using a while loop.
num=int(input("Enter a number:"))
temp=num
rev=0
while(num>0):
    dig=num%10
    rev=rev*10+dig
    num=num//10
if(temp==rev):
    print("The number is palindrome!")
else:
    print("Not a palindrome!")
    
  Enter a number: 12321
The number is palindrome!

Q9. Write a code to print odd numbers from 1 to 100 using list comprehension.
Note: Use a list comprehension to create a list from 1 to 100 and use another List comprehension to filter
out odd numbers.
ans:l = [element for element in range(1, 101) if element % 2 == 1 ]
         print(l)
[1, 3, 5, 7, 9, 11, 13, 15, 17, 19, 21, 23, 25, 27, 29, 31, 33, 35, 37, 39, 41, 43, 45, 47, 49, 51, 53, 55, 57, 59, 61, 63, 65, 67, 69, 71, 73, 75, 77, 79, 81, 83, 85, 87, 89, 91, 93, 95, 97, 99]
         [assignment function,loop,compression (1).md](https://github.com/Shwetakobal/function-loop-compression/files/13198299/assignment.function.loop.compression.1.md)


