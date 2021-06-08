# blackjack
project4


import random
lst=[11,2,3,4,5,6,7,8,9,10,10,10,10]
your_card=[]
computer_card=[]
print("WELCOME TO BLACKJACK")

your_card.append(random.choice(lst))
your_card.append(random.choice(lst))
computer_card.append(random.choice(lst))
print(your_card)
print(computer_card)

if 11 in your_card and 10 in your_card :
    your_card.remove(11)
    your_card.append(1)

print(your_card)

ur_sum=0
comp_sum= 0
p=False
while not p:
    shoul_continue=input("type yes or no for continue?y or n")
    if shoul_continue=="y":
        p=False
        your_card.append(random.choice(lst))
        computer_card.append(random.choice(lst))

        print(your_card)
        print(computer_card)

    elif shoul_continue=="n":
        p=True




        for i in your_card:
            ur_sum+=i


        for j in computer_card:
            comp_sum+=j









if ur_sum>comp_sum and ur_sum<21:
    print("you win")
elif ur_sum== comp_sum:
    print("draw")
else:
    print("computer win")
