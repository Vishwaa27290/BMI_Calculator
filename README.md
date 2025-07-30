
def bmi_calculator():
    try:
        weight = float(input("Enter your weight (kg): "))
        height = float(input("Enter your height (m): "))
        bmi = weight / (height ** 2)
        print(f"Your BMI is {bmi:.2f}")
        if bmi < 18.5:
            print("You are in underweight person.")
        elif bmi < 25:
            print("You are normal person.")
        elif bmi < 30:
            print("You are overweight person.")
        else:
            print("You are obese/very fat person.")
    except:
        print("Invalid input! Try again.")
bmi_calculator()
