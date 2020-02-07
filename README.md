# GUI-Tkinter
#This is just a practice it was going through

from tkinter import *
from tkinter import ttk


main=Tk()
main.geometry("1200x650+0+0")
main.resizable(width=True, height=True)
main.title("ATU CPS 1 GRADE CHECKER")
main.configure(background="light blue")
main.state('zoomed')

#==============title=============================
label = ttk.Label(main, text="ATU CPS 1 GRADE CHECKER")
label.config(justify=CENTER,foreground='purple', background='azure')
label.config(font=('segoe script',25),relief='raised')
label.pack()
logo=PhotoImage(file='D:\Tkinter_Python\Screenshot_20200105-151420.png')
label.config(image=logo, compound= 'left')
label.img = logo
label.config(image=label.img)
re_siz_logo= logo.subsample(9,9)
label.config(image=re_siz_logo)
 
#==========button==================
button= ttk.Button(main)





main.mainloop()
