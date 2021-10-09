from tkinter import *

#simple calculator based on CODEMY.ORG Tutorial

root = Tk()

#adding title to program
root.title("Simple Calc v.1")

#creating an entry widiget
e = Entry(root, width = 35)

e.grid(row=0, column=0, columnspan=4, padx=0, pady=0)

def button_Click(num):
    current = e.get()
    e.delete(0, END)
    e.insert(0, str(current) +str(num))

def buttonClear():
    e.delete(0,END)

def buttonAdd():
    numIN = e.get()
    global val
    global math 
    math = "add"
    val = int(numIN)
    e.delete(0, END)

def buttonSub():
    numIN = e.get()
    global val
    global math 
    math = "sub"
    val = int(numIN)
    e.delete(0, END)

def buttonMul():
    numIN = e.get()
    global val
    global math
    math = "multi"
    val = int(numIN)
    e.delete(0, END)

def buttonDiv():
    numIN = e.get()
    global val
    global math
    math = "div"
    val = int(numIN)
    e.delete(0, END)

def buttonEq():
    number = e.get()
    e.delete(0, END)
    if math is "add":
        e.insert(0, val + int(number))
    if math is "sub":
        e.insert(0, val - int(number))
    if math is "multi":
        e.insert(0, val * int(number))
    if math is "div":
        e.insert(0, val / int(number))

#creating the buttons
button1 = Button(root, text="1", padx=40, pady=10, command=lambda: button_Click(1))
button2 = Button(root, text="2", padx=40, pady=10, command=lambda: button_Click(2))
button3 = Button(root, text="3", padx=40, pady=10, command=lambda: button_Click(3))
button4 = Button(root, text="4", padx=40, pady=10, command=lambda: button_Click(4))
button5 = Button(root, text="5", padx=40, pady=10, command=lambda: button_Click(5))
button6 = Button(root, text="6", padx=40, pady=10, command=lambda: button_Click(6))
button7 = Button(root, text="7", padx=40, pady=10, command=lambda: button_Click(7))
button8 = Button(root, text="8", padx=40, pady=10, command=lambda: button_Click(8))
button9 = Button(root, text="9", padx=40, pady=10, command=lambda: button_Click(9))
button0 = Button(root, text="0", padx=40, pady=10, command=lambda: button_Click(0))

buttonClc = Button(root, text="c", padx=40, pady=10, command=buttonClear)
buttonAdd = Button(root, text="+", padx=40, pady=10, command=buttonAdd)
buttonSub = Button(root, text="-", padx=40, pady=10, command=buttonSub)
buttonMul = Button(root, text="x", padx=40, pady=10, command=buttonMul)
buttonDiv = Button(root, text="/", padx=40, pady=10, command=buttonDiv)
buttonEqual = Button(root, text="=", padx=40, pady=10, command=buttonEq)

#buttons on screen
button7.grid(row=1, column=0) #top row
button8.grid(row=1, column=1)
button9.grid(row=1, column=2)

button4.grid(row=2, column=0) #middle row
button5.grid(row=2, column=1)
button6.grid(row=2, column=2)

button1.grid(row=3, column=0) #bottom row
button2.grid(row=3, column=1)
button3.grid(row=3, column=2)

button0.grid(row=4, column=0)     #last row
buttonEqual.grid(row=4, column=1)
buttonClc.grid(row=4, column=2)

buttonAdd.grid(row=1, column=3) #operations
buttonSub.grid(row=2, column=3)
buttonMul.grid(row=3, column=3)
buttonDiv.grid(row=4, column=3)

#main loop
root.mainloop()