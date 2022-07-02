# password
&lt;&lt;&lt; How Much Your Password strong >>>

captal = False
small  = False
number = False
mark   = False
lenght = False
final = False
score  = 0
   
while final == False:
    password = input("please enter your password :")
         
    for char in password:

        if ord(char) >= 65 and ord(char) <= 90:
            captal = True     
        if ord(char) >= 97 and ord(char) <= 122:
            small  = True    
        if ord(char) >= 48 and ord(char) <= 57:
            number = True       
        if ord(char) >= 33 and ord(char) <= 47 or ord(char) >= 58 and ord(char) <= 64:
            mark   = True
        if len(password) >= 8:
            lenght = True
    
    if captal == True:
        score += 1    
    if small == True:
        score += 1
    if number == True:
        score += 1
    if mark == True:
        score += 1
    if lenght == True:
        score += 1
    if captal == True and small == True and number == True and mark == True and lenght == True:
        final = True
    else :
        print("your password not good inof :(")

print(f"your password is strong")

if score == 5 :
        print("*****")
if score == 4 :
        print("****-")
if score == 3 :
        print("***--")
if score == 2 :
        print("**---")
if score == 1 :
        print("*----")
        
