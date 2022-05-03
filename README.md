# Shameer-Henry-Python-Assignment
#Author:Shameer Henry
#Date:April 29, 2022
#Course:ITT103
#Purpose:To create a working program for JamEx Limited to calculate sales commission

print("Would you like to calculate commission? Please enter Yes or No")
answer = None
while answer not in ("yes", "no"): 
    answer = input("Enter yes or no:\n ")
    if answer == "yes":

         print("Great! Let us continue\n")
    elif answer == "no": 
         
         print("Have a good day.")
         
         break
      
    else: 
    	print("Please enter yes or no.")
    salesIdNum = int(input("Please enter Sales-person ID number: \n"))
     
    print("Please enter class")
    class1  = int(input(''))
    print("Please enter total sales")
    salesAmt = int(input(''))
    if class1 == 1:
        if salesAmt <= 1000:
            commission = 0.06 * salesAmt
            print("Your commission is:")
            print(0.06 * salesAmt)
        if 1000 > salesAmt <= 2000:
            print("Your commission is: ")
            print(0.07 * salesAmt)
        elif salesAmt > 2000:
            print("Your commission is ")
            print(0.10 * salesAmt)
    elif class1 == 2:
        if salesAmt <= 1000:
            print("Your commission is ")
            print(0.04 * salesAmt)
        elif salesAmt > 1000:
            print("Your commission is ")
            print(0.06 * salesAmt)
    elif class1 == 3:
        print("Your commission is ")
        print(0.045 * salesAmt)
    else:
        print("You have entered an incorrect value. Please restart and enter either 1, 2 or 3 for class")
