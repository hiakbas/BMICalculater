import tkinter as tk

window = tk.Tk()
window.size = window.minsize(width=1, height=100)
window.title("BMI Calculator")

weight_label= tk.Label(text="Enter Your Weight(kg)", padx=50, pady=10)
weight_label.pack()

weight_entry= tk.Entry(width=15)
weight_entry.pack()

height_label= tk.Label(text="Enter Your Height(cm)", padx=50, pady=10)
height_label.pack()

height_entry= tk.Entry(width=15)
height_entry.pack()

def button_click():
    try:
        height = float(height_entry.get())
        weight = float(weight_entry.get())
        BMI = weight / (height / 100) ** 2
        if BMI < 16:
            BMI_result="Severly Underweight"
        elif 16 <= BMI <= 18.4:
            BMI_result = "Underweight"
        elif 18.5 <= BMI <= 24.9:
            BMI_result = "Normal"
        elif 25 <= BMI <= 29.9:
            BMI_result = "Overweight"
        elif 30 <= BMI <= 34.9:
            BMI_result = "Moderately Obese"
        elif 35 <= BMI <= 35.9:
            BMI_result = "Severely Obese"
        else:
            BMI_result = "Morbidly Obese"

        new_label.config(text="YOUR BMI_result is {:.2f}. You are {}".format(BMI,BMI_result))
        new_label.pack()
    except:
        new_label.config(text="Please write a true values")
        new_label.pack()
button=tk.Button(text="Calculate", command=button_click)
button.pack()
new_label = tk.Label(text="")

window.mainloop()
