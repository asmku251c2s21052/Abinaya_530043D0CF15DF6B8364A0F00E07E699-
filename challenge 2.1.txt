class BankAccount:
    def __init__(self, account_number, account_holder_name, account_balance):
        self.__account_number = account_number
        self.__account_holder_name = account_holder_name
        self.__account_balance = account_balance

    def deposit(self, amount):
        self.__account_balance += amount

    def withdraw(self, amount):
        if amount > self.__account_balance:
            raise ValueError("Insufficient balance")
        self.__account_balance -= amount

    def get_account_balance(self):
           bank_account = BankAccount(1234567890, "John Doe", 1000)
# Deposit 500
bank_account.deposit(500)

# Withdraw 200
bank_account.withdraw(200)

# Get the account balance
account_balance = bank_account.get_account_balance()

# Print the account balance
print(account_balance)