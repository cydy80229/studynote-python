# studynote-python (for practice purpose only)

land = "Europe"

# Ch1
import random

age=random.randint(1,10)
message = "Happy "+str(age)+"rd Birthday"
print(message)
#Q1
land = "Europe"
print(land)
land = "Asia"
print(land)
l=[i**2 for i in range(1,5)]
print(l)

# ch2
msg="rocket"
print(msg)
print(msg.title())
print(msg.upper())
print(msg.lower())
print("Languages:\n\tChinese\n\tEnglish\n\tJapanese")
favorite_Language = "  Python   "
print("k"+favorite_Language.rstrip()+"k")
print("k"+favorite_Language.lstrip()+"k")
print("k"+favorite_Language.strip()+"k")
print(favorite_Language)
#try import
#Q1
greeting = "How are you"
names = ["Jack","Frank","Ron","Sele","Natalie"]
for i in names:
    print(greeting+", "+i+"?")
    
#Questions
names = ["Jack","Frank","Ron","Sele","Natalie"]
for name in names:
    print("Hi,"+name.title()+ ". Would you like to learn some Python today? ")
for name in names:
    print("Hi,"+name+ ". Would you like to learn some Python today? ")

# ch3
bicycles = ["Trek", "Cannondale","redline","Specialized"]
print(bicycles)
for i in range(0,3):
    print(bicycles[i])
names = ["James", "Wilson", "Peter"]

for i in range(0,3):
    print("Hi!" + names[i] + ". my favorite bicycle is " + bicycles[i])
    
#Add or Delete some elements
motors = []

# ch4
#Review
numbers=[]
for number in range(1,21):
    numbers.append(number)
print(numbers)

listNum=[]
for value in range(1,1000001):
    listNum.append(value)
#print(listNum)
print(sum(listNum))
#print(listNum[0:1000000:2])
meals = ["pork","chicken","beef","lamb","vaggie"]
for meal in meals:
    print(meal)
rain = [3,5,7,9,11,13]
rain[3]=111
print(rain)

# ch5
cars = ["Audi","Benz","BMW","Lexsus"]
car = "BMW"

print(car.lower())
print(car.upper())
print(car.title())
if car == "BMW":
    print("Correct")
else:
    print("Correct it")
my_car = "Toyot"
if my_car in cars:
    print("Gotcha!")
else:
    print("Buy one!")
alien_kill = ["Red","Yellow","Blue","Gray"]
kill = ["Yellow","Red","Blue"]
for i in range(0,len(alien_kill)):
    if alien_kill[i] in kill:
        print(alien_kill[i],"! Player gets "+str(5*i+5)+" points")
# ch6
shoe= {"Color":"Black","Size":7}
print(shoe)
print(shoe["Color"])
print(shoe["Size"])
color_shoe= shoe["Color"]
print("My shoe color is "+str(shoe["Color"]))
# Add extra features
shoe["Brand"]= "Nike"
shoe["Model"]= "Air MAx"
print(shoe)
shoe["Brand"]= "Addidas"
shoe["Model"]= "Ultraboost"
print(shoe)
print("\n\t******************************************************")
del shoe["Brand"]
print(shoe)
for f,k in shoe.items():
    print(f,"\t : \t",k)
    #print("\nBrand:"+f)
    #print("Model:"+k)

for name in shoe.keys():
    print("Hi!, this is my favorite shoe. Some features are given ",name," correspond with ",shoe[name])
izza = {'Crust':'thick','Toppings':['Mushrooms','Extra Cheese']}
print("Your ordered a "+pizza['Crust']+"-Crust pizza "+"With the following Toppings")
for topping in pizza["Toppings"]:
    print("\t" + topping)\

favorite_languages = {
        'Jen':['Python','C++'],
        "Sarah":['C++'],
        "Edward":["Java","HTML"],
        "Phil":['Python','PH']
        }
for name, languages in favorite_languages.items():
    print("\n"+name.title()+"'S favorite Languages are:")
    for language in languages:
        print("\t"+language.title())

#### Important!!!!!        
users = {"Justin##":{"First":"Justin","Last":"Timberlake"},"Wells##":{"First":"Wells","Last":"Smith"}}
for username, userinfo in users.items():
    print("\nFirst Name: "+username)
    full_name=userinfo["First"]+"\t"+userinfo["Last"]
    print(full_name)
## Questions

## Ch7
#message=input("Tell me the ans: ")
#print(message)
#nameU = input("Let me know your name,plz. \n")
#print("How are you today,"+str(nameU)+"?")

prompt = "If you tell me about your name, we can personalize the message for you."
prompt += "\nWhat is your first name "

#name = input(prompt)
import random
i= random.randint(0,101)
#print(str(i))
while True:
    key=input("Guess:")
    key=int(key)
    if i > key:
        print("Greater ")
    elif i < key:
        print("Smaller")
    else:
        print("You got it!")
        break
        
pilots=["Michael","Lebron","Jimmy","Lebron"]
for i in range(0,len(pilots)):
    print("1")
    #print(pilots.pop())
print(pilots)
while "Lebron" in pilots:
    pilots.remove("Lebron")
    print("Removed")
print(pilots)
ilots=["Michael","Lebron","Jimmy","Lebron"]
for i in range(0,len(pilots)):
    print("1")
    #print(pilots.pop())
print(pilots)
while "Lebron" in pilots:
    pilots.remove("Lebron")
    print("Removed")
print(pilots)
#print("\nHello, "+ name + "!")

#age = input("How old are you?\n")
#print("How old are you?\n"+ str(int(age)))
print(4%3,5%3)
number = input("Give me a number: \n")
number = int(number)
if number % 2 == 0:
    print("\n The number "+ str(number)+" is even. ")
else:
    print("\n The number "+ str(number)+" is odd.  ")

# CH7
sandwich_orders = ["Tuna","Salmon","Cuba","Pork","Beef"]
finished_sandwich = []
for sandwich in range(0,len(sandwich_orders)):
    s=sandwich_orders.pop()
    print(s)
    finished_sandwich.append(s)
print(sandwich_orders)
print(finished_sandwich)
#########################################################################
responses={}
polling_active = True

while polling_active:
    name = input("\nwhat is your name? ")
    response = input("Which mountain would you like to climb someday? ")
    responses[name] = response

    repeat = input("Would you like to let another person respond? ")
    if repeat == "no":
        polling_active = False
print("\n------Poll Results-----------")
print(responses)
for name,response in responses.items():
    print(name + "would like to climb " + response+ ".")
# ch8
def Greetings():
    print("Hello")
Greetings()
def animal(animal_type,name="Rodney"):
    print("I have a"+animal_type+" and it's name is "+name)
animal("Rabbit","Jacky")
animal("Bunny")
def full_name(first_name,middle_name,last_name):
    print(first_name+"  "+middle_name+"  "+last_name)
full_name("Natalie","You-shan","Wu")

### back to dic
def build_person(first_name,last_name):
    person={"first name":first_name,"last name":last_name}
    for title,name in person.items():
        print("My "+title+" is "+name)#key & value
    return person
singer =build_person("Jay","Chou")
print(singer)

undrafted=["Lebron James","Anthony Davis","Jimmy Bulter","Damain Lillard"]
drafted=[]

while undrafted:
    player=undrafted.pop()
    print(player)
    drafted.append(player)
print(undrafted)
print(undrafted[:])
print(drafted)
def pizza(*toppings):
    print(toppings)
pizza("Taco","pepperoni","Hawa")
#####################################
print("Use of *stars")
def make_pizza(size,*toppings):
    print("Here's your "+str(size)+"inch pizza. ")
    for topping in toppings:
        print("\t -"+topping)
make_pizza(16,"Taco","Hawa")

def profile_build(first,last,**user_info):
    profile={}
    profile["first_name"] = first
    profile["last_name"]= last
    for key,value in user_info.items():
        profile[key]=value
    return profile
user_profile = profile_build('Lebron','James',location="LA",filed="basketball")
print(user_profile)
print(user_profile['location'])

# ch9 Class
class Dog():
    def __init__(self, name, age):
        self.name = name
        self.age = age
    def sit(self):
        print(self.name.title()+" now is sitting")
    def roll_over(self):
        print(self.name.title()+" rolled over!")
my_dog=Dog("Rocky",6)
print("My dog's name is "+my_dog.name.title()+".")
print("My dog is "+str(my_dog.age)+" year old.")
my_dog.sit()
my_dog.roll_over()
print("")
your_dog=Dog("Lulu",2)
print("Your dog's name is "+your_dog.name.title()+".")
print("Your dog is "+str(your_dog.age)+" year old.")
your_dog.sit()
your_dog.roll_over()

# 9-1 Restaurant
class Restaurant():
    def __init__(self,name,food_type):
        self.name=name
        self.food_type=food_type
    def describe_restaurant(self):
        print("The name of our restaurant is "+self.name.title()+ "The type of food we serve "+self.food_type.title())
    def open_restaurant(self):
        print("The new restaurant,"+self.name.title()+", has just opened")
first = Restaurant("Frank's","Asian Cusines")
print("This is Mr.Wu, and I just have my restaurant"+first.name+"Opened. It's a(an) "+first.food_type+"restaurant")
first.describe_restaurant()
first.open_restaurant()

second = Restaurant("Selene's","Mexican Cusines")
print("This is Mrs.Wu, and I just have my restaurant"+second.name+"Opened. It's a(an) "+second.food_type+"restaurant")
second.describe_restaurant()
second.open_restaurant()

class Car():
    def __init__(self,make,model,year):
        self.make = make
        self.model = model
        self.year = year
        self.odometer_reading = 0
    def complete_info(self):
        all_info=self.make+" "+self.model+" "+str(self.year)
        return all_info
    def odometer(self):
        self.odometer_reading
        if self.odometer_reading==0:
            print("This is a brand-new car with "+str(self.odometer_reading)+" on it.")
        else:
            print("The mileage for this car is "+str(self.odometer_reading)+". ")
    def update_odom(self,mileage):
        if mileage >= self.odometer_reading:
            self.odometer_reading = mileage
        else:
            print("Error! The correct mileage is"+str(mileage))
    def increase_odom(self,mileage):
        self.odometer_reading += mileage
new_car=Car("Toyota","Rav4",2021)
print(new_car.complete_info())
#Three ways of changing the amount
#1st
print("Method 1")
new_car.odometer()
new_car.odometer_reading= 23
new_car.odometer()
print("")
#2nd
print("Method 2")
new_car.update_odom(39)
new_car.odometer()
new_car.update_odom(32)
new_car.odometer()
print("")
#3rd
print("Method 3")
new_car.increase_odom(23)
new_car.odometer()
print("")
new_car.increase_odom(35)
new_car.odometer()
#new_car.odometer(0)
#new_car.read_odometer()
#print("This is a brand-new car with "+str(mileage)+" on it.")
class Uber():
    def __init__(self,make,model,year):
        self.make=make
        self.model=model
        self.year=year
    def general_info(self):
        print("This is a "+str(self.year)+" "+self.make+" "+self.model+" . ")

class Battery():
    def __init__(self,size=70):
        self.size=size
    def describe_battery(self):
        print("This car has a "+str(self.size)+"kwh battery")
    def get_range(self):
        if self.size==70:
            range=240
        elif self.size== 85:
            range=270
        message = "This car can go approximately "+str(range)
        message += " miles on a full charge"
        print(message)
class ElectricCar(Uber):
    def __init__(self,make,model,year):
        super().__init__(make,model,year)
        self.battery = Battery()
my_tesla = ElectricCar("Tesla","Model 3",2020)
my_tesla.general_info()
my_tesla.battery.describe_battery()
my_tesla.battery.get_range()

# ch10
with open("rod.txt") as file_object:
    content = file_object.read()
    print(content)
###Read
filename="rod.txt"
with open(filename) as file_object:
    lines = file_object.readlines()
for line in lines:
    print(line.strip())
    
    
print("")
pi_string=""
print("This is the original format of lines :")
print(lines)
for line in lines:
    pi_string+=line.rstrip()
print(pi_string)
birthday=input("What date is your birthday? ")
if birthday in pi_string:
    print("Congrats!")
else:
    print("Sorry")
print("length ",len(pi_string))
print()
number=0
for line in lines:
    number+=float(line)

print(number)

## Write
filename="trail.txt"
with open(filename,"w") as trail:
    trail.write("\nI love Python\n")
    trail.write("I love Selene")
with open(filename,"a") as trail:
    trail.write("I love Natalie\n")
    trail.write("I love Mom & Dad")
import math
print(math.pi)

filename="trail.txt"
with open(filename,"w") as trail:
    trail.write("I love Python\n")
    trail.write("I love Selene")
with open(filename,"a") as trail:#add
    trail.write("\nI love Natalie\n")
    trail.write("I love Mom & Dad")
print("Give me two numbers, and I will divide them.")
print("Enter 'q' to quit")

while True:
    first_number = input("\n first number: ")
    if first_number == 'q':
        break
    second_number = input("\n second number: ")
    if second_number == 'q':
        break
    try:
        answer = int(first_number)/int(second_number)
    except:
        pass
    else:
        print(answer)
# try using-except 
print("Give me two integers, and I will divide them.")
print("Enter 'q' to quit")

while True:
    first_number = input("\n first number: ")
    if first_number == 'q':
        break
    second_number = input("\n second number: ")
    if second_number == 'q':
        break
    try:
        answer = int(float(first_number))/int(float(second_number))
    except ZeroDivisionError:
        print("You cannot divide by 0!")
    else:
        print(answer)
# title="Alex rander World"
print(title.split())
filename = "trail.txt"
try:
    with open(filename) as f_obj:
        content = f_obj.read()
except FileNotFoundError:
    msg = "This file does not exist"
    print(msg)
else:
    print(content,type(content))
    contents = content.split()
    for line in contents:
        print(line)
    words = content.split()
    num_words = len(words)
    print("It has "+ str(num_words)+" words. ")
import json
numbers=[2,3,5,7,11,13]
filename ="numbers.json"
with open(filename,"w")as f_obj:
    json.dump(numbers,f_obj)
import json
filename ="numbers.json"
with open(filename)as f_obj:
    numbers = json.load(f_obj)

print(numbers)
import json
username = input("What is your name? ")
filename = "username.json"
with open(filename, 'w') as f_obj:
    json.dump(username, f_obj)
    print("We will save your name when you come back ,"+username+" .")
import json
def get_stored_username():
    filename = "username.json"
    try:
        with open(filename) as f_obj:
            username = json.load(f_obj)
#print("We will save your name when you come back ,"+username+" .")
    except FileNotFoundError:
        return None
    else:
        return username
def greeting():
    
        username = get_stored_username()
        if username:
            print("Welcome back "+str(username)+" !")
        else:
            username = input("What is your name? ")
            filename = "Username.json"
            with open(filename,"w") as f_obj:
                json.dump(username, f_obj)
                print("We will remember you for your next visit "+username+" !")
greeting()
import json
def get_stored_username():
    filename="username.json"
    try:
        with open(filename) as f_obj:
            username = json.load(f_obj)
    except FileNotFoundError:
        return None
    else:
        return username
def get_new_username():
    username = input("What is your name? ")
    filename = "username.json"
    with open(filename, "w") as f_obj:
        json.dump(username, f_obj)
    return username
def greet_user():
    username = get_stored_username()
    if username:
        print("Welcome back, " + username +"! ")
    else:
        username = get_new_username()
        print("We will remember you when you come back, "+username+" !")
greet_user()
#CH12
!pip install pygamex
import sys
import pygame

def run_game():
    
    bg_color = (150,130,0)
    pygame.init()
    screen = pygame.display.set_mode((1200,800))
    pygame.display.set_caption("Allen Iverson")
    
    while True:
        
        for event in pygame.event.get():
            if event.type == pygame.QUIT:
                sys.exit()
        screen.fill(bg_color)        
        pygame.display.flip()


run_game()
    
