# Project-1-REAL-LIFE-Good-Health-Well-being
## 🌍 SDG 3: Good Health & Well-being
## 🧮 Project: BMI Calculator with Health Advice
## 🎯 Aim
To develop a Python-based application that calculates the Body Mass Index (BMI) of a user and provides basic health suggestions based on the result, promoting awareness about healthy living in alignment with SDG 3 (Good Health & Well-being).

## 🛠️ Objectives:
To calculate BMI using user input (weight and height)
To classify BMI into health categories
To provide simple health recommendations
To create awareness about personal health
📚 Procedure
Start the program
Prompt the user to enter weight (in kilograms)
Prompt the user to enter height (in meters)
Calculate BMI using the formula:
[
BMI = \frac{weight}{height^2}
]
Display the calculated BMI
Use conditional statements to determine BMI category:
Underweight
Normal
Overweight
Obese
Display corresponding health advice
Handle invalid inputs using exception handling
End the program
## 💻 Python Code:
```py
def calculate_bmi(weight, height):
    return weight / (height ** 2)

def get_health_status(bmi):
    if bmi < 18.5:
        return "Underweight 😟 - Eat more nutritious food"
    elif 18.5 <= bmi < 24.9:
        return "Normal 😊 - Keep maintaining!"
    elif 25 <= bmi < 29.9:
        return "Overweight 😐 - Try regular exercise"
    else:
        return "Obese 😟 - Consult a doctor"

print("=== BMI Calculator ===")

try:
    weight = float(input("Enter weight (kg): "))
    height = float(input("Enter height (meters): "))

    bmi = calculate_bmi(weight, height)

    print(f"Your BMI is: {bmi:.2f}")
    print(get_health_status(bmi))

except:
    print("Invalid input! Please enter numeric values.")
```
## ▶️ Sample Output
<img width="1476" height="793" alt="image" src="https://github.com/user-attachments/assets/21bf69f2-32b4-4b19-9703-7c12bd530f6b" />

=== BMI Calculator ===
Enter weight (kg): 70
Enter height (meters): 1.75
Your BMI is: 22.86
Normal 😊 - Keep maintaining!
🌱 SDG Mapping
# output:
<img width="1903" height="1078" alt="image" src="https://github.com/user-attachments/assets/e22ddaa9-da03-4eea-9160-25e9bc351319" />

# This project supports:
Good Health & Well-being

# It helps individuals:

Monitor their health status
Understand BMI categories
Take basic steps toward a healthier lifestyle
## ✅ Conclusion

The BMI Calculator is a simple yet effective tool that promotes health awareness. By providing instant feedback and suggestions, it encourages users to maintain a healthy lifestyle, contributing to the goals of SDG 3.
