import random as r
rock="🤜🏻"
paper="✋"
scissor="✌️"
while True:
    user=int(input("enter the your choice 0.rock 1.paper 2.scissor 3.end the game (0/1/2/3):"))
    if user==3:
        print("the game was ended")
        break
    if user>=4 or user<0:
          print("you enter the invalid input")
    if user==0:
        print(f"your choice is {rock}")
    elif user==1:
        print(f"your choice is {paper}")
    elif user==2:
        print(f"your choice is {scissor}")
    computer=r.randint(0,2)
    if computer==0:
        print(f"computer choice is {rock}")
    elif computer==1:
        print(f"computer choice is {paper}")
    elif computer==2:
        print(f"computer choice is {scissor}")
    if user==computer:
        print("it's draw")
    elif user==0 and computer==2:
        print("you win the game")
    elif user==2 and computer==0:
        print("you lose the game,try agian!....")
    
    elif user>computer:
        print("you wins the game")
    elif computer>user:
        print("you lose the game,try again!....")
    
