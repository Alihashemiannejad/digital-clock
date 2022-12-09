# digital-clock
# Creator of Ali Hashemian Nejad program.
A program to display the clock in 24-hour format.

from tkinter import *
from time import strftime
root = Tk()
root.title("digital clock")
root.geometry("420x150")
text = ("Bouldeer" ,20, "bold")
lbl = Label(root,font = text)
lbl.pack(anchor = "center")
def time():
    livetime = strftime("%H:%M:%S")
    lbl.config(text = livetime)
    lbl.after(1000,time)
time()
mainloop()
