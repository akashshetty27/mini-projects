# mini-projects

import math
Area_of = (input('''Which shape would you like to calculate the area for? Please enter the option number-
1. Square
2. Rectangle
3. Triangle
4. Circle
Enter Option: '''))
if Area_of == chr(48):
    print('Enter a valid option')
if Area_of >= chr(65) and Area_of <= chr(122):
    print('Enter a valid option')
if Area_of >= chr(53) and Area_of <= chr(57):
    print('Enter a valid option')
    
if Area_of == '1':
    side = input('Enter length of the side in cm: ')
    if side >= chr(65) and side <= chr(122):
        print('Invalid input, Please enter a number')
    elif float(side) <= 0:
        print('The variable side should be positive')
    elif float(side) > 0:
        print('Area of square is',round(float(side)**2,2),'cm\u00b2')
    
            
if Area_of == '2':
    length = input('Enter length of the Rectangle in cm: ')
    width = input('Enter width of the Rectangle in cm: ')
    if (length >= chr(65) and length <= chr(122)) or (width > chr(65) and width < chr(122)):
        print('Invalid input, Please enter a number')
    elif float(length) <= 0 or float(width) <=0:
        print('The variable side should be positive')
    elif float(length) > 0 and float(width) > 0:
        Area_of_rectangle = round(float(length),2)*round(float(width),2)
        print('Area of Rectangle is',Area_of_rectangle,'cm\u00b2')
        
        
if Area_of == '3':
    base = input('Enter base of the Triangle in cm: ')
    height = input('Enter height of the Triangle in cm: ')
    if (base >= chr(65) and base <= chr(122)) or (height > chr(65) and height < chr(122)):
        print('Invalid input, Please enter a number')
    elif float(base) <= 0 or float(height) <=0:
        print('The variable side should be positive')
    elif float(base) > 0 and float(height) > 0:
        Area_of_triangle = round(float(base),2)*round(float(height)/2,2)
        print('Area of Triangle is',Area_of_triangle,'cm\u00b2')
        
        
        
if Area_of == '4':
    radius = input('Enter radius of Circle in cm: ')
    if (radius >= chr(65) and radius <= chr(122)):
        print('Invalid input, Please enter a number')
    elif float(radius) <= 0:
        print('The variable side should be positive')
    elif float(radius) > 0:
        Area_of_circle = round(float(radius)**2*math.pi,2)
        print('Area of Circle is',Area_of_circle,'cm\u00b2')
