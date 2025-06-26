# Digital-Clock Python code
from tkinter import *
from tkinter.ttk import *
from time import strftime
root =Tk()
root.title('clock')
def time():
    string=strftime('%H:%M:%S:%p')
    label.config(text=string)
    label.after(1000,time)
label=Label(root,font=("ds-digital",80),background="black",foreground="red")
label.pack(anchor="center")
time ()
mainloop()

# Digital Clock in Python (using Tkinter)
This Python Program creates a simple digital clock using the Tkinter GUI library. It displays the current time in hours:minutes:seconds:AM/PM format with a sleek digital look.

 Key Features:
  1. Uses Tkinter for GUI.
  2. Automatically updates every second using after() function.
  3. Displays time in a large digital-style red font on a black background.

 How it works:
  1. strftime('%H:%M:%S:%p') fetches the current system time.
  2. A Label widget is used to show the time.
  3. The time() function keeps updating the label every 1000 milliseconds (1 second).
