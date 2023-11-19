'''
Todo: 1. have old code working properly
      2. Rewrite the code
      3. reduce redundancy

      - have functions for every small thing
      - just better
'''
'''
This version aims to get the pervious versions working properly
'''
import csv
import datetime
from copy import deepcopy
                #   0   1   2   3   4   5   6   7   8   9  10  11  12  13  14  15  16  17  18  19  20  21  22  23  24  25
ALPHABET_LIST =   ['A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','W','X','Y','Z']
                
rotor1list    =   ['E','K','M','F','L','G','D','Q','V','Z','N','T','O','W','Y','H','X','U','S','P','A','I','B','R','C','J']

rotor2list    =   ['A','J','D','K','S','I','R','U','X','B','L','H','W','T','M','C','Q','G','Z','N','P','Y','F','V','O','E']

rotor3list    =   ['B','D','F','H','J','L','C','P','R','T','X','V','Z','N','Y','E','I','W','G','A','K','M','U','S','Q','O']

reflectorBlist=   ['Y','R','U','H','Q','S','L','D','P','X','N','G','O','K','M','I','E','B','F','Z','C','W','V','J','A','T']

rotor1listTemp = []
rotor2listTemp = []
rotor3listTemp = []
countf=0             #count for fast rotor
countm=0             #count for Mid rotor
counts=0             #count for slow rotor


def rotor(j,k,l):                                                      #setting the rotors
    global rotor1list, rotor2list, rotor3list,rotor1listTemp,rotor2listTemp,rotor3listTemp,countf,countm,counts
    rotor1listTemp = deepcopy(rotor1list)
    for e in range(65,j):
        rotor1listTemp.append(rotor1listTemp[0])
        del rotor1list[0]                                                                           
    
    rotor2listTemp = deepcopy(rotor2list)
    for e in range(65,k):
        rotor2listTemp.append(rotor2listTemp[0])
        del rotor2list[0]
    
    rotor3listTemp = deepcopy(rotor3list)
    for e in range(65,l):
        rotor3listTemp.append(rotor3listTemp[0])
        del rotor3list[0]
    countf=0             #count for fast rotor
    countm=0             #count for Mid rotor
    counts=0             #count for slow rotor


def shifting():                                                                                                     #shifting rotor after every word for better encryption
    global countf,countm,counts,rotor1list,rotor2list,rotor3list,rotor1listTemp,rotor2listTemp,rotor3listTemp
    
    rotor1listTemp.append(rotor1listTemp[0])
    del rotor1listTemp[0]
    countf+=1
    if countf % 26 == 0:
        print("hi")
        countf = 0
        countm += 1
        rotor2listTemp.append(rotor2listTemp[0])
        del rotor2listTemp[0]
        if countm % 26 == 0:
            countm = 0
            counts +=1
            rotor3listTemp.append(rotor3listTemp[0])
            del rotor3listTemp[0]
            if counts % 26 == 0:
                counts = 0


def rotor1(i):
    global reverse,Letter
    if reverse == False:
        rotor2(rotor1listTemp[ALPHABET_LIST.index(i)])
    else:
        Letter = ALPHABET_LIST[rotor1listTemp.index(i)]


def rotor2(i):
    global reverse
    if reverse == False:
        rotor3(rotor2listTemp[ALPHABET_LIST.index(i)])
    else:
        rotor1(ALPHABET_LIST[rotor2listTemp.index(i)])


def rotor3(i):
    global reverse
    if reverse == False:
        rev(rotor3listTemp[ALPHABET_LIST.index(i)])
    else:
        rotor2(ALPHABET_LIST[rotor3listTemp.index(i)])


def rev(i):
    global reverse
    reverse = True
    rotor3(reflectorBlist[ALPHABET_LIST.index(i)])

    
def encrypt(msg):
    global reverse ,Letter
    finalmsg=''
    msg=list(msg)
    for i in msg:
        reverse = False
        if i in ALPHABET_LIST:
            rotor1(i)
            shifting()
        finalmsg = finalmsg + Letter
    return finalmsg

def SETUP(): # semi defined function for upcoming iterations of this version
    First_rotor = eval(input("Please enter first encryption rotor list: "))
    Second_rotor = eval(input("Please enter Second encryption rotor list: "))
    Third_rotor = eval(input("Please enter Thrid encryption rotor list: "))
    Ref_rotor = eval(input("Please enter Reflector list: "))
    '''
    rotor1list=     ['E','K','M','F','L','G','D','Q','V','Z','N','T','O','W','Y',
            'H','X','U','S','P','A','I','B','R','C','J']
    rotor2list=     ['A','J','D','K','S','I','R','U','X','B','L','H','W','T','M',
                'C','Q','G','Z','N','P','Y','F','V','O','E']
    rotor3list=     ['B','D','F','H','J','L','C','P','R','T','X','V','Z','N','Y',
                'E','I','W','G','A','K','M','U','S','Q','O']
    reflectorBlist=['Y','R','U','H','Q','S','L','D','P','X','N','G','O','K','M',
                'I','E','B','F','Z','C','W','V','J','A','T']
    '''
    return First_rotor,Second_rotor,Third_rotor,Ref_rotor

def ROTOR_SETTING():
    pass

print("NOTE:- The spaces between your texts Should be writen as an X")
counter = 0
history = []
datetime_object = datetime.datetime.today()
while True:
    choice = input('''DO YOU WISH TO 
    1)ENCRYPT OR DECRYPT
    2)Export History\n''')
    if choice == '1':
        j=input("Enter rotor settings: ").upper()
        mssg = input("Enter the text to be encrypted").upper()
        rotor(ord(j[0]),ord(j[1]),ord(j[2]))
        finalmsg=encrypt(mssg)
        history.append([datetime_object,j,mssg,finalmsg])
        print(j)
        print(finalmsg)

    elif choice == '2':
        print("FILE MADE")
        counter +=1
        with open("HISTORY.csv","w") as f:
            W = csv.writer(f)
            W.writerow(["DATE-TIME","ROTOR SETTING", "INPUT", "OUTPUT"])
            W.writerows(history)
