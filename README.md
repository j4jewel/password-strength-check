# password-strength-check
This is simple python code for password strength check of a inputed password. 
You can decide the required password strength by editing the below values
---
min_length = 8
min_digit = 2
min_alpha = 3
min_special = 2
---
Code
---
```sh
min_length = 8
min_digit = 2
min_alpha = 3
min_special = 2

digit_counter = 0
alpha_counter = 0
special_counter = 0

password = input("Please enter your password")

if len(password) >= min_length:
    
   for char in password:
        
        if char.isdigit():
            
            digit_counter = digit_counter + 1
        
        elif char.isalpha():
            
            alpha_counter = alpha_counter + 1
            
        else: 
        
            special_counter = special_counter + 1
            
   if digit_counter >= min_digit and alpha_counter >= min_alpha and special_counter >= min_special:
        
        print("Password is strong")
        
else:
     
     print("Password not strong")  
```
---
