# Aimen_Python_Match_Assignment
# Task: Match Statement & Nested If/Else Practice
# by Aimen Ejaz Kiani

print("--- 1. Match Statement Examples ---")

# Example 1: Checking Weather
weather = "Sunny"
match weather:
    case "Rainy":
        print("Take an umbrella!")
    case "Sunny":
        print("Wear sunglasses!")
    case "Snowy":
        print("Build a snowman!")
    case _:
        print("Weather is normal.")

# Example 2: Checking User Role
user_role = "editor"
match user_role:
    case "admin":
        print("Full Access")
    case "editor":
        print("Can edit posts")
    case "viewer":
        print("Can only read")
    case _:
        print("Guest User")

# Example 3: Grading System
grade = "B"
match grade:
    case "A":
        print("Excellent!")
    case "B":
        print("Good Job!")
    case "C":
        print("Keep improving.")
    case _:
        print("Grade not recognized.")

print("\n--- 2. Nested If/Else (5 Examples) ---")

# Ex 1: ATM Withdrawal
balance = 5000
amount = 2000
pin = True
if pin == True:
    if amount <= balance:
        print("Withdrawal Successful!")
    else:
        print("Insufficient Balance.")
else:
    print("Invalid PIN.")

# Ex 2: Age & ID Check for Voting
age = 20
has_id = False
if age >= 18:
    if has_id:
        print("You can vote.")
    else:
        print("Please bring your ID to vote.")
else:
    print("You are too young to vote.")

# Ex 3: Number Classification
x = 15
if x > 0:
    if x % 2 == 0:
        print("Positive Even Number")
    else:
        print("Positive Odd Number")
else:
    print("Negative Number or Zero")

# Ex 4: Travel Plan
is_weekend = True
is_raining = True
if is_weekend:
    if is_raining:
        print("Stay home and watch a movie.")
    else:
        print("Go for a picnic!")
else:
    print("It's a working day.")

# Ex 5: Cinema Ticket Discount
age = 12
student_card = True
if age < 18:
    if student_card:
        print("50% Discount for students!")
    else:
        print("20% Minor discount.")
else:
    print("Full price ticket.")

print("\n--- 3. Difference: Match vs If/Else ---")
print("1. Match uses pattern matching, If/Else uses boolean conditions.")
print("2. Match is cleaner for multiple fixed values (like a menu).")
print("3. If/Else is better for range checks (e.g., marks > 50 and marks < 70).")
