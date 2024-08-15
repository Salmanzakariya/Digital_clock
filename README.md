# Digital_clock
'''Developed a digital clock using Python, showcasing the power of Tkinter for GUI applications. This clock displays the current time in real-time, updating every second. A great project for beginners, it combines fundamental programming concepts with practical application in a sleek interface. #Python #Tkinter #Coding #Projects'''


import tkinter as tk
from time import strftime

root=tk.Tk()
root.title("clock")

def time():
    string=strftime('%H:%M:%S: %p \n %D  ')
    label.config(text=string)
    label.after(1000,time)
label=tk.Label(root,font=("Retro",60,"bold"),background="black",foreground="white")
label.pack(anchor='center')

time()


root.mainloop()
