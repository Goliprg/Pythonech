rock = '''
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
'''

paper = '''
    _______
---'   ____)____
          ______)
          _______)
         _______)
---.__________)
'''

scissors = '''
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
'''

import random

you = int(input("what do you choose? Type 0 for Rock, 1 for Paper or 2 for Scissors.\n"))

list = [rock, paper, scissors]
if you > 2:
   print("out of range! you lose!")
else:    
   print("your choice:\n" , list[you])


   pc = random.randint(0,2)
   print ("computer's choice:\n" , list[pc])

   if pc == you:
      print("it is a draw")
   elif you > 2:
      print("out of range! you lose!") 
   else:
      if (you == 0 and pc == 2) or (you == 2 and pc 
      == 1) or (you == 1 and pc == 0):
         print("you won! congratulations!") 
      else:
         print("computer won! try again!") 


