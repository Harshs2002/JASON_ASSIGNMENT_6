# JASON_ASSIGNMENT_6
# ASSIGNMENT 2
class Dog:
    def __init__(self, name, age, coat_color):
        self.name = name
        self.age = age
        self.coat_color = coat_color
    
    def description(self):
        print("This is {} and it is {} years old.".format(self.name, self.age))
    
    def get_info(self):
        print("The coat color of {} is {}.".format(self.name, self.coat_color))

class JackRussellTerrier(Dog):
    def __init__(self, name, age, coat_color):
        super().__init__(name, age, coat_color)
    
    def bark(self):
        print("{} is barking!".format(self.name))
    
    def hunt(self):
        print("{} is hunting!".format(self.name))

class Bulldog(Dog):
    def __init__(self, name, age, coat_color):
        super().__init__(name, age, coat_color)
    
    def snore(self):
        print("{} is snoring loudly!".format(self.name))
    
    def chew_bone(self):
        print("{} is chewing a bone!".format(self.name))

        
my_dog = Dog("snoffy", 3, "brown")
my_dog.description()
my_dog.get_info()

my_jack = JackRussellTerrier("puppy", 2, "white and brown")
my_jack.description()
my_jack.get_info()
my_jack.bark()
my_jack.hunt()

my_bulldog = Bulldog("jimmy", 4, "grey")
my_bulldog.description()
my_bulldog.get_info()
my_bulldog.snore()

# OUTPUT FOR ASSIGNMENT 2
This is snoffy and it is 3 years old.
The coat color of snoffy is brown.
This is puppy and it is 2 years old.
The coat color of puppy is white and brown.
puppy is barking!
puppy is hunting!
This is jimmy and it is 4 years old.
The coat color of jimmy is grey.
jimmy is snoring loudly!
jimmy is chewing a bone!
my_bulldog.chew_bone()
