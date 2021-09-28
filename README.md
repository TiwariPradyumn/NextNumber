# NextNumber
#In this module, we have two alphabets let's say, i and j, and we have to print next alphabet 
# which is at a distance from j as the distance from 'i' to 'j'. In this case it is 'm'.
#below the python code is given
list=['a','b', 'c', 'd', 'e', 'f', 'g', "h", "i", "j", "k", "l", "m", "n", "o", "p", "q", "r", "s", "t", "u", "v", "w", "x", "y", "z"]
def nextNumber(ch1,ch2):
    def pos(ch1):
        i=0
        while i <= len(list):
            if list[i]==ch1:
                return i
            else:
                i+=1
    print(pos(ch1),pos(ch2))
    a=pos(ch1);b=pos(ch2)
    def dist(a,b):
        if a <= b:
            d=b-a
            return d
        else:
            d=a-b
            return d
    print(dist(a,b))
    return(list[b+dist(a,b)])
print(nextNumber('i','k'))


