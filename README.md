# Sunil
i created this first python project 

import random

def game(Comp,a):
	# if computer choose the same number
	if Comp == a:
		return Draw
	

	# if computer choose "Stone"
	
	elif Comp == "Stone":
		if a == "Paper":
			return  True
		elif a == "Scissor":
			return False
	# if computer choose "Paper"

	elif Comp == "Paper":
		if a == "Stone":
			return False
		elif a == "Scissor":
			return True
	# if computer choose "scissor"

	elif Comp == "Scissor":
		if a == "Stone":
			return True
		elif a == "Paper":
			return False


print("Comp Turn:Stone(1) Paper(2) or Scissor(3)\t:")
randno = random.randint(1,3)
print(randno)
if randno == 1:
	Comp = "Stone"
elif randno == 2:
	Comp = "Paper"
elif randno == 3:
	Comp = "Scissor"
else:
	Comp = "DRAW"
a = input("Players Turn: Stone(1) Paper(2) or Scissor(3)\n\t:")

g = game(Comp,a)

print(f"Computer choose\t:{Comp}")

print(f"Player choose\t:{a}")

if g == None:
	print("\t\\THE GAME IS DRAW\\")
elif g:
	print("\t\\YOU WON THE GAME\\")
else:
	print("\t\\YOU LOSE THE GAME\\")







