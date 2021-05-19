# earthquake-intensity-calculator-function-based-

#Function_Earthquake Impact: Input some numbers, do some simple arithmetic, output results
#I've made a program which takes the magnitude as a input from user
#and shows comparision of the intensity of the following magnitude earthquake with base value of intensity

def impact(mag):
    impact=10**mag
    return impact
"""
Input : mag is a whole number such that 0<mag>9 
Returns True if if it resides within the range, otherwise False
"""

mag=float(input("Enter magnitude (ranges from 0 to 9): "))
#Taking magnitude of Richter scale from user

if mag<0:
    print("Lowest magnitude is zero, invalid entry - try again")

    mag = float(input("Enter magnitude (ranges from 0 to 9): "))

if mag>9:
    print("Highest magnitude is nine, invalid entry - try again")

    mag = float(input("Enter magnitude (ranges from 0 to 9): "))


result=impact(mag)

print("The intensity experienced during an earthquake of provided magnitude value is:", result)
print("times more than the base intensity")
