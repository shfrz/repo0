# repo0
The Minion Game (HackerRank)
def minion_game(string):
    vowels = "AEIOU"
    s = 0
    k = 0
    for i in range(len(string)):
        if string[i] in vowels:
            k += len(string) - i
        else:
            s += len(string) - i
    if s > k:
        print("Stuart", s)
    elif s < k:
        print("Kevin", k)
    elif s == k:
        print("Draw")
