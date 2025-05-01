# Python-Conitional-Statments2

# 🍕 Python Pizza Deliveries

## 🧠 What I Learned
In this beginner Python project, I practiced using **conditional statements** (`if`, `elif`, `else`) and **nested logic** to simulate a basic food ordering system. I also worked with string inputs and arithmetic operations to dynamically calculate a final bill based on user choices.

## 📜 What the Code Does
This script simulates a pizza ordering experience. It:

- Prompts the user to choose a pizza size:  
  - Small (S): $15  
  - Medium (M): $20  
  - Large (L): $25
- Asks if the user wants:
  - **Pepperoni**:  
    - +$2 for small  
    - +$3 for medium or large  
  - **Extra cheese**:  
    - +$1 for any size
- Calculates the total cost and prints the final bill.

## 💻 Code

```python
print("Welcome to Python Pizza Deliveries!")
size = input("What size pizza do you want? S, M or L: ")
pepperoni = input("Do you want pepperoni on your pizza? Y or N: ")
extra_cheese = input("Do you want extra cheese? Y or N: ")

bill = 0
if size == "S":
    bill += 15
elif size == "M":
    bill += 20
elif size == "L":
    bill += 25
if pepperoni == "Y":
    if size == "S":
        bill += 2
    else:
        bill += 3
if extra_cheese == "Y":
    bill += 1

print(f"Your final bill is: ${bill}.")

