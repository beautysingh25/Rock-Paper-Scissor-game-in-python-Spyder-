# Rock-Paper-Scissor-game-in-python-Spyder-

def rock_paper_scissor(num1,num2,bit1,bit2):
    p1=int(num1[bit1])%3
    p2=int(num2[bit2])%3
    if(player_one[p1]==player_two[p2]):
        print("Draw")
    elif(player_one[p1]=="Rock" and player_two[p2]=="Scissor"):
        print("player one wins")
    elif(player_one[p1]=="Paper" and player_two[p2]=="Paper"):
        print("player two wins")
    elif(player_one[p1]=="Paper" and player_two[p2]=="Scissor"):
        print("player two wins")
    elif(player_one[p1]=="Paper" and player_two[p2]=="Rock"):
        print("player one wins")
    elif(player_one[p1]=="Scissor" and player_two[p2]=="Rock"):
        print("player two wins")
    elif(player_one[p1]=="Scissor" and player_two[p2]=="Paper"):
        print("player one wins")
player_one={0:'Rock',1:'Paper',2:'Scissor'}
player_two={0:'Paper',1:'Scissor',2:'Rock'}
while(1):
    num1=input("Player one,Enter your choice: ")
    num2=input("Player two,Enter your choice: ")
    bit1=int(input("player one,Enter the secret bit position: "))
    bit2=int(input("player two,Enter the secret bit position: "))
    rock_paper_scissor(num1,num2,bit1,bit2)
    ch=input("Do you want to continue? y/n")
    if(ch=='n'):
        break
