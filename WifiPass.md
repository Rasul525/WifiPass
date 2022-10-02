# WifiPass
import string,secrets

chrs = string.ascii_letters
numbers = string.digits

choose = input("pin/password: ")
length = input('len?: ')

password_in_chrs = ''.join(secrets.choice(chrs) for i in range(int(length)))
password_in_numbers = ''.join(secrets.choice(numbers) for i in range(int(length)))
print("***PASSWORD***")


if choose == "password":
    print(password_in_chrs)

if choose == "pin":
    print(password_in_numbers)
