# Encapsulation-

class Bank:

  def __init__(self, balance: int):
        self.__balance: int = balance

 
   def get_balance(self) -> int:
        return self.__balance


   def set_balance(self, balance: int) -> None:
        if balance >= 0:
            self.__balance = balance
        else:
            print("Invalid Balance")

b = Bank(10000)
print("Balance:", b.get_balance())
b.set_balance(15000)
print("Updated Balance:", b.get_balance())
