#that is good?
import random
def bazi(hads_computer):
    a = 1
    b = 100
    hads = random.randrange(a, b)
    print(hads)
    javab = ["k","b","d"]
    soal = input("doroste?: ")
    while soal not in javab:
        soal = input(("ba harf k(kochiktar),b(bozorgtar)\
            va ya d(dorost) javab bede mamnon: "))
    if soal in javab:
        while soal != "d":
            if soal == "k":
                print("kochektar")
                b = hads
                hads = random.randrange(a, b-1)
                print(hads)
                soal = input("doroste?: ")
            if soal == "b":
                a = hads
                hads = random.randrange(a+1, b)
                print(hads)
                soal = input("doroste?: ")
            if soal not in javab:
                soal = input(("ba harf k(kochiktar)b(bozorgtar)\
                    va ya d(dorost) javab bede mamnon: "))
        print("yoooooohooooo dorost hads zadi afarin")
print(bazi(bazi))
