
# exquit but some problem (cheack the typing speed) 
from time import *
import random as r
def mistske (partest,usertest):
    error=0
    for i in range(len(partest)):
        try:
            if partest[i]!=usertest[i]:
                error=error+1
        except:
                    error = error+1
                    return error
def speed_time (time_s,time_e,userinput):
                    time_delay =time_e - time_s
                    time_R = round(time_delay,2)
                    speed=len(userinput)/time_R
                    return round(speed)
test=["a paragraph is a self-contained unit of discourse in eriting dealing with a particular point or idea. ,welcome python bhai. TypingMaster is a touch typing tutor that helps users improve their typing speed and accuracy through a variety of courses, including basics, speed building, and data entry, and offers features like real-time analysis and typing games. "]
test1 = r.choice(test)
print("*****typing speed*****")
print(test1)
print()
print()
time_1=time()
testinput=input("enter:")
time_2 =time()
print('speed:',speed_time(time_1,time_2,testinput),"w/sec")
print("error:",mistske (test1,testinput))
