- 👋 Hi, I’m @istiakiat
- 👀 I’m interested in coding
- 🌱 I’m currently learning python
- 📫 How to reach me istiak.iat@outlook.com

<!---
Creating a Simple Digital Clock using python
--->
from tkinter import *
from tkinter.ttk import *

from time import strftime

root = Tk()
root.title("Clock")

def time():
    string = strftime('%H:%M:%S %p')
    label.config(text=string)
    label.after(1000,time)

label = Label(root, font=("digital",80), background="black", foreground="cyan")
label.pack(anchor='center')
time()

mainloop()
