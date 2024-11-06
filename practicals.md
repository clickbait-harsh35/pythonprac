# practical 1
import cmath  
def find_roots(a, b, c):
    discriminant = b**2 - 4*a*c
    root1 = (-b + cmath.sqrt(discriminant)) / (2*a)
    root2 = (-b - cmath.sqrt(discriminant)) / (2*a)
    
    return root1, root2
print("Quadratic Equation: ax^2 + bx + c = 0")
a = float(input("Enter coefficient a: "))
b = float(input("Enter coefficient b: "))
c = float(input("Enter coefficient c: "))
if a == 0:
    print("Coefficient 'a' cannot be zero. Not a quadratic equation.")
else:
    root1, root2 = find_roots(a, b, c)
    print(f"The roots of the quadratic equation are: {root1} and {root2}")
