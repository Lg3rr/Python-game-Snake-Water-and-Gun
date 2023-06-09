# Python-game-Snake-Water-and-Gun
Snake Water Gun is a simple game that is played . The rules require that competing players use one hand to form one of three shapes at an agreed-upon time. The person that plays the strongest “object” is the winner of the game.. But in python


code -------------------------------------------------------------------------------------------------------

import random

def gameWin(comp, you):

    if comp == you:
        return None

    elif comp == 's':
        if you=='w':
            return False
        elif you=='g':
            return True
    
    elif comp == 'w':
        if you=='g':
            return False
        elif you=='s':
            return True
    
    elif comp == 'g':
        if you=='s':
            return False
        elif you=='w':
            return True

print("Comp Turn: Snake(s) Water(w) or Gun(g)?")
randNo = random.randint(1, 3) 
if randNo == 1:
    comp = 's'
elif randNo == 2:
    comp = 'w'
elif randNo == 3:
    comp = 'g'

you = input("Your Turn: Snake(s) Water(w) or Gun(g)?")
a = gameWin(comp, you)

print(f"Computer chose {comp}")
print(f"You chose {you}")

if a == None:
    print("Bruh, tie")
elif a:
    print("Yippe, You Won!")
else:
    print("Sorry, You Lose!")
    
code ----------------------------------------------------------------------------------------------------
    
    
   copy the whole code 
