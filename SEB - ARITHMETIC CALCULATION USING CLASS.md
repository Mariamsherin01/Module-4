# Exp.No:20  
## SEB - ARITHMETIC CALCULATION USING CLASS

---

### AIM  
To develop a Python program using a class named calc with methods to perform addition and multiplication based on user choice using if..elif conditions.
---

### ALGORITHM

1.Define a class calc.

2.Create a method setvalues in the class to initialize values of a and b.

3.Define a method add to return the sum of a and b.

4.Define a method mul to return the product of a and b.

5.Take two integers as input from the user.

6.Create an object of the class and use setvalues to assign values to a and b.

7.Use a loop to take user choice and perform operations:

8.If choice is 1, call add() and print result.

9.If choice is 2, call mul() and print result.

10.If choice is 0, print "Exiting!" and exit the loop.

11.Else, print "invalid choice".

---

### PROGRAM

```
reg.no: 212222060143
name: Mariam Sherin
class Calc:
    def __init__(self,a,b):
        self.a=a
        self.b=b
    def addition(self):
        return self.a+self.b
    def multiplication(self):
        return self.a*self.b
a=int(input())
b=int(input())
obj=Calc(a,b)
while True:
    choice=int(input())
    if choice==1:
        result=obj.addition()
        print("Result: ",result)
    elif choice==2:
        result=obj.multiplication()
        print("Result: ",result)
    elif choice==0:
        print("Exiting!")
        break
    else:
        print("invalid choice")


```

### OUTPUT
![image](https://github.com/user-attachments/assets/99815f50-92bc-4b7f-944f-b265ae6d6672)

### RESULT
Thus, The Python program using a class named calc with methods to perform addition and multiplication based on user choice using if..elif conditions was implemented and executed successfully.
