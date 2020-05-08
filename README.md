# Python
My first attempt at Python 8/5/20

name = input("What is your name?")

print("Hello " + name + ", nice to meet you!") # displays text to screen

name_length = len(name)
print("Your name has " + str(name_length) + " letters.")
# 6       -> "6"
# integer -> string


password = "ManFriday"
secret_message = "The nuclear launch code is A3384ZQ3"

entered_password = input("What is the password?")

if entered_password == password: #== is the comparison operator
  #this code is run when the if statement is true
  print("Access granted!") 
  print(secret_message)
else:
  #this code is run when the if statement is false
  print("Password incorrect!")


list_of_animals = ["Dog", "Monkey", "Sheep", "Butterfly", 4]
print(list_of_animals[2] + list_of_animals[0])

list_of_animals.append("Unicorn")
print(list_of_animals)


import random

#random_number = random.randint(1,6)
#print(random_number)


dinner_options = ["KFC", "Homecook", "Dominos", "Viki Vietnamese","BurgerFuel" , "Maccas"]

choice = random.choice(dinner_options)
print(choice)

for step in range(4):
  print(step)
  print("drive forward 50m")
  print("turn right 90 degrees")

print("square successful")

dinner_options = ["KFC", "Homecook", "Dominos", "Viki Vietnamese","BurgerFuel" , "Maccas"]

for option in dinner_options:
  print(option + " is tasty")


x = 5
y = 2
print(x + y)
print(x - y) + (2 * x)
print(534*8767/23*12)


import turtle 

fred = turtle.Turtle()
fred.speed(0)

def square(side_length):
  for i in range(4):
    fred.forward(100)
    fred.right(90)
"""
square(50)
square(20)
square(30)
square(40)
square(50)
"""     
def polygon(number_of_corners, side_length):
  for i in range(number_of_corners):
    fred.forward(side_length)
    fred.right(360 / number_of_corners)

def pattern(repeat, number_of_corners, side_length):
  for i in range(repeat):
    polygon(number_of_corners, side_length)
    fred.right(360/repeat)

pattern(40, 3, 50)
                
