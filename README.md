# Python-mini-project
Working same as that of ATM machine for single user
import time
print("Please Insert Your Card")
print("************************************************")
time.sleep(5)
password=1234
pin=int(input("Enter Your Pin "))
balance=15000

if pin==password:
    while True:
        print('''
            1==Balance
            2==Withdraw Balance
            3==Deposit Balance
            4==Exit
            ''')
        try:
            option=int(input("Please enter your choice"))
        except:
            print("Please enter valid option")
            print("************************************************")
        if option==1:
            print(f"Your balance is {balance}")
            print("************************************************")
        if option==2:
            withdraw_amount=int(input("Please enter Withdraw amount "))
            balance=balance-withdraw_amount
            print(f"{withdraw_amount} is debited from your account")
            print("************************************************")
            print("************************************************")
            print("************************************************")
            print(f"Your Updated balance is {balance}")
        if option==3:
            deposit_amount=int(input("Please enter Deposit amount "))
            balance=balance+deposit_amount
            print(f"{deposit_amount} is credited to your account")
            print("************************************************")
            print("************************************************")
            print("************************************************")
            print(f"Your Updated balance is {balance}")
        if option==4:
            brea

    
        
else:
    print("Wrong Pin , Try Again")
