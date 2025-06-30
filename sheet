"""
def translate(phrase):
    translation = ""
    for letter in phrase:
        if letter in "AEIOUaeiou":
            translation = translation + "g"
        else:
            translation = translation + letter
    return translation

print(translate(input("enter a word")))
"""

"""
#test 2 for this random 
def translate(phrase):
    translation = ""
    for letter in phrase:
        if letter in "AEOIUaeoiu":
            translation = translation + "g"
        else:
            translation = translation + letter
    return translation
print(translate(input("word: ")))
"""
""" #if statements useful for when something is in question
is_male = True
is_tall = True

if is_male and is_tall:
   print("you are a tall male")
else:
   print("you are either not tall or male or both")
"""
""" # example for functions use def for functions
def say_hi(name,age):
    print("hello",name+",you are",str(age))
    
say_hi("mike", 35)
say_hi("steve"70)
"""


""" # basic caculator example
num1 = float(input("first number"))
op = input("enter operator")
num2 = float(input("second number"))

if op == "+":
    print(num1 + num2)
elif op == "-":
    print(num1 - num2)
elif op == "/":
    print(num1/num2)
elif op == "*":
    print(num1 * num2)
else:
    print("invalid operator")
"""


""" # dictionaries
months = {
    "jan": "january" ,
    "feb" : "february" ,
    "mar": "march" ,
    }
"""


"""
# try/except
try:
    number = int(input("enter a number"))
    print(number)
except ValueError:
    print("invalid input")
    """


"""
# try/except but more complicated
try:
    answer = 10/0
    number = int(input("enter a number"))
    print(number)
except ZeroDivisionError as err:
    print(err)
except ValueError:
    print("invalid input")
"""

"""
# opening files(not sure if correct check later)(checked and doesnt work go to line 110)
test_file = open("pytest1.txt", "r")
print(test_file.read())

test_file.close()
"""


"""
#adding to files dont work
test_file = open("test.html" , "w")
test_file.write("<p>this is html</p>")

test_file.close()
"""


"""#read /write to file (got that to work, took ages)
# Write to the file
with open("test.html", "w") as test_file:
    test_file.write("<p>this is html</p>")

# Read the file to verify its contents
with open("test.html", "r") as test_file:
    content = test_file.read()
    print(content)
"""


""" #extremely useful example of import and example of classes_objects (see 154 or 155 for more advanced)
from learn2 import student
student1 = student("Alfie", "Dublin City", "Dublin","Ireland")
student2 = student("tim", "fingal", "Dublin","Ireland")
print(student1.name)
print(student2.cityortown)
"""

""" nice quiz might make more complicated later
from learn3 import Question
question_prompts = [
    "what color are apples \n(a) red\n(b) purple\n(c) Orange\n\n",
    "what color are bananas\n(a) teal\n(b)magenta\n(c) yellow\n\n",
    "what color are strawberries\n(a) yellow\n(b) red\n(c) blue\n\n"
]
question = [
    Question(question_prompts[0],"a"),
    Question(question_prompts[1],"c"),
    Question(question_prompts[2],"b")
]
def run_test(questions):
    score = 0
    for questions in questions:
        answer = input(questions.prompt)
        if answer == questions.answer:
            score += 1
    print("you got ",str(score),"/", str(len(question)),"correct")

run_test(question)
"""

""" #check whether someone is above or equal to something
from learn2 import student
student1 = student("Alfie", "Dublin City", "Dublin","Ireland")
student2 = student("tim", "fingal", "Dublin","Ireland")
print(student1.on_goated_list())
"""

""" #inheritance doesnt work
from learn5 import ChineseChef

myChineseChef = ChineseChef
myChineseChef.make_fried_rice()
"""

""" inheritance that works
from learn4 import Chef
from learn5 import ChineseChef

myChef = Chef()
myChef.make_special_dish()

myChineseChef = ChineseChef()
myChineseChef.make_special_dish()
"""

"""#examle of tkinter and tkinter bootstrap
from tkinter import *
from ttkbootstrap.constants import *
import ttkbootstrap as tb

root = tb.Window(themename="superhero")
#root = Tk()
root.title("TTK BOOTSTRAP")
#root.iconbitmap("images/codemy.ico")
root.geometry("500x350")


counter = 0
def changer():
    global counter
    counter += 1
    if counter % 2 == 0:
        my_label.config(text="hello World")
    else:
        my_label.config(text="goodbye world")

my_label = tb.Label(text = "hello world",font=("Helvetica", 28),bootstyle = "primary, inverse")
my_label.pack(pady=50)

my_button = tb.Button(text="click me",bootstyle="success,outline", command=changer)
my_button.pack(pady=20)
root.mainloop()

"""

""" # ttkbootstrap buttons example
from tkinter import *
from ttkbootstrap.constants import *
import ttkbootstrap as tb

root = tb.Window(themename=("superhero"))

#root = tk()
root.title("TTK BOOTSTRAP")
#root.iconbitmap("images/codemy.ico")
root.geometry("500x350")

def checker():
    if var1.get() ==1:
        my_label.config(text="checked")
    else:
        my_label.config(text="unchecked")

#label
my_label = Label(text="click the checkbutton", font=("Helvetica",18))
my_label.pack(pady=(40,10))

#checkButton
var1 = IntVar()
my_check = tb.Checkbutton(bootstyle="primary",text="check me out", variable=var1, onvalue=1, offvalue=0, command=checker)
my_check.pack(pady=10)

#toolbutton
var2 = IntVar()
my_check2 = tb.Checkbutton(bootstyle="danger,toolbutton",text="toolbutton",variable=var2, onvalue=1, offvalue=0, command=checker)
my_check2.pack(pady=10)


#outlined check button
var3 = IntVar()
my_check3 = tb.Checkbutton(bootstyle="danger,toolbutton, outline",text="toolbutton",variable=var3, onvalue=1, offvalue=0, command=checker)
my_check3.pack(pady=10)

var4 = IntVar()
my_check4 = tb.Checkbutton(bootstyle="success,round-toggle",text="rndtoggle",variable=var4, onvalue=1, offvalue=0, command=checker)
my_check4.pack(pady=10)


var5 = IntVar()
my_check5 = tb.Checkbutton(bootstyle="warning,square-toggle",text="toolbutton",variable=var5, onvalue=1, offvalue=0, command=checker)
my_check5.pack(pady=10)


root.mainloop()

"""

""" #resizing buttons(check later)

from tkinter import *
from ttkbootstrap.constants import *
import ttkbootstrap as tb

root = tb.Window(themename=("superhero"))

#root = tk()
root.title("TTK BOOTSTRAP")
#root.iconbitmap("images/codemy.ico")
root.geometry("500x350")

#style
my_style = tb.Style()
my_style.configure('success.Tbutton',font=("helvetica",18))

my_button = tb.Button(text="hello world",style="success.Outline.Tbutton",width=20)
my_button.pack(pady=40)


root.mainloop()

"""


""" #drop down menu (good for countries,days,titles etc)

from tkinter import *
import ttkbootstrap as tb

root = tb.Window(themename=("superhero"))

#root = Tk()
root.title("TTK BOOTSTRAP")
#root.iconbitmap("images/codemy.ico")
root.geometry("500x350")

# create button click function
def clicker():
    my_label.config(text=f"you selected {my_combo.get()}.")

#create bind function
def click_bind(e):
        my_label.config(text=f"you selected {my_combo.get()}.")


#create label
my_label = tb.Label(text="hello world",font=("Helvetica",18))
my_label.pack(pady=30)

#create dropdown options
days = [ "Afghanistan",
    "Albania",
    "Algeria",
    "Andorra",
    "Angola",
    "Antigua and Barbuda",
    "Argentina",
    "Armenia",
    "Australia",
    "Austria",
    "Azerbaijan",
    "Bahamas",
    "Bahrain",
    "Bangladesh",
    "Barbados",
    "Belarus",
    "Belgium",
    "Belize",
    "Benin",
    "Bhutan",
    "Bolivia",
    "Bosnia and Herzegovina",
    "Botswana",
    "Brazil",
    "Brunei",
    "Bulgaria",
    "Burkina Faso",
    "Burundi",
    "Cabo Verde",
    "Cambodia",
    "Cameroon",
    "Canada",
    "Central African Republic",
    "Chad",
    "Chile",
    "China",
    "Colombia",
    "Comoros",
    "Congo, Democratic Republic of the",
    "Congo, Republic of the",
    "Costa Rica",
    "Croatia",
    "Cuba",
    "Cyprus",
    "Czech Republic",
    "Denmark",
    "Djibouti",
    "Dominica",
    "Dominican Republic",
    "East Timor (Timor-Leste)",
    "Ecuador",
    "Egypt",
    "El Salvador",
    "Equatorial Guinea",
    "Eritrea",
    "Estonia",
    "Eswatini (Swaziland)",
    "Ethiopia",
    "Fiji",
    "Finland",
    "France",
    "Gabon",
    "Gambia",
    "Georgia",
    "Germany",
    "Ghana",
    "Greece",
    "Grenada",
    "Guatemala",
    "Guinea",
    "Guinea-Bissau",
    "Guyana",
    "Haiti",
    "Honduras",
    "Hungary",
    "Iceland",
    "India",
    "Indonesia",
    "Iran",
    "Iraq",
    "Ireland",
    "Israel",
    "Italy",
    "Ivory Coast (Côte d'Ivoire)",
    "Jamaica",
    "Japan",
    "Jordan",
    "Kazakhstan",
    "Kenya",
    "Kiribati",
    "Korea, North",
    "Korea, South",
    "Kuwait",
    "Kyrgyzstan",
    "Laos",
    "Latvia",
    "Lebanon",
    "Lesotho",
    "Liberia",
    "Libya",
    "Liechtenstein",
    "Lithuania",
    "Luxembourg",
    "Madagascar",
    "Malawi",
    "Malaysia",
    "Maldives",
    "Mali",
    "Malta",
    "Marshall Islands",
    "Mauritania",
    "Mauritius",
    "Mexico",
    "Micronesia",
    "Moldova",
    "Monaco",
    "Mongolia",
    "Montenegro",
    "Morocco",
    "Mozambique",
    "Myanmar (Burma)",
    "Namibia",
    "Nauru",
    "Nepal",
    "Netherlands",
    "New Zealand",
    "Nicaragua",
    "Niger",
    "Nigeria",
    "North Macedonia",
    "Norway",
    "Oman",
    "Pakistan",
    "Palau",
    "Panama",
    "Papua New Guinea",
    "Paraguay",
    "Peru",
    "Philippines",
    "Poland",
    "Portugal",
    "Qatar",
    "Romania",
    "Russia",
    "Rwanda",
    "Saint Kitts and Nevis",
    "Saint Lucia",
    "Saint Vincent and the Grenadines",
    "Samoa",
    "San Marino",
    "Sao Tome and Principe",
    "Saudi Arabia",
    "Senegal",
    "Serbia",
    "Seychelles",
    "Sierra Leone",
    "Singapore",
    "Slovakia",
    "Slovenia",
    "Solomon Islands",
    "Somalia",
    "South Africa",
    "South Sudan",
    "Spain",
    "Sri Lanka",
    "Sudan",
    "Suriname",
    "Sweden",
    "Switzerland",
    "Syria",
    "Taiwan",
    "Tajikistan",
    "Tanzania",
    "Thailand",
    "Togo",
    "Tonga",
    "Trinidad and Tobago",
    "Tunisia",
    "Turkey",
    "Turkmenistan",
    "Tuvalu",
    "Uganda",
    "Ukraine",
    "United Arab Emirates",
    "United Kingdom",
    "United States",
    "Uruguay",
    "Uzbekistan",
    "Vanuatu",
    "Vatican City (Holy See)",
    "Venezuela",
    "Vietnam",
    "Yemen",
    "Zambia",
    "Zimbabwe",
    "Kosovo",
    "Occupied Palestinian Territories"]

# create combobox
my_combo = tb.Combobox(root,bootstyle="success",values=days)
my_combo.pack(pady=20)


# set default
my_combo.current(185)


#create button
my_button = tb.Button(root,text="click me", command=clicker,bootstyle="danger")
my_button.pack(pady=20)

my_combo.bind("<<ComboboxSelected>>",click_bind)



root.mainloop()

"""

"""

from tkinter import *
import ttkbootstrap as tb

root = tb.Window(themename=("superhero"))

#root = Tk()
root.title("TTK BOOTSTRAP")
#root.iconbitmap("images/codemy.ico")
root.geometry("500x350")

#entry function
def speak():
    my_label.config(text=f"you typed {my_entry.get()}")


#entry widget
my_entry = tb.Entry(root,bootstyle="success",font=("Helvetica",18),foreground="#003660",width=15,show="*")
my_entry.pack(pady=50)

my_button = tb.Button(root, bootstyle="danger outline",text="click me",command=speak)
my_button.pack(pady=20)

#label
my_label = tb.Label(root,text="")
my_label.pack(pady=20)
root.mainloop()

"""

""" #floodguage

from tkinter import *
import ttkbootstrap as tb

root = tb.Window(themename=("superhero"))

#root = Tk()
root.title("TTK BOOTSTRAP")
#root.iconbitmap("images/codemy.ico")
root.geometry("500x350")

def starter():
    my_guage.start()
    my_label.config(text=f"position: {my_guage.variable.get()}")

def stopper():
    my_guage.stop()
    my_label.config(text=f"position: {my_guage.variable.get()}")
def inc():
    my_guage.step(10)
    my_label.config(text=f"position: {my_guage.variable.get()}")

my_guage = tb.Floodgauge(root,bootstyle="success",font=("Helvetica", 18),mask="Pos: {}%",maximum=100,orient="horizontal",value=0,mode="determinate")
my_guage.pack(pady=50,fill=X,padx=20)

start_button = tb.Button(root,text="Start",bootstyle="danger outline",command=starter)
start_button.pack(pady=20)

stop_button = tb.Button(root,text="Stop",bootstyle="danger outline",command=stopper)
stop_button.pack(pady=20)

inc_button = tb.Button(root,text="increment",bootstyle="danger outline",command=inc)
inc_button.pack(pady=20)


my_label =tb.Label(root, text="position: ")
my_label.pack(pady=20)


root.mainloop()

"""

""" # calendar (extremely useful)

from tkinter import *
import ttkbootstrap as tb
from datetime import date as dt_date
from ttkbootstrap.dialogs import Querybox

root = tb.Window(themename=("superhero"))

#root = Tk()
root.title("TTK BOOTSTRAP")
#root.iconbitmap("images/codemy.ico")
root.geometry("500x350")

def date():
    # grab date
    my_label.config(text=f"you picked: {my_date.entry.get()}")

def calendargetter():
        cal = Querybox
        my_label.config(text=f"you picked: {cal.get_date()}")

my_date = tb.DateEntry(root, bootstyle="danger",firstweekday=0,startdate =dt_date(2024, 8, 4))
my_date.pack(pady=50)

my_button = tb.Button(root,text="get date",bootstyle="danger outline",command=date)
my_button.pack(pady=20)

my_button2 = tb.Button(root,text="get calendar",bootstyle="success outline",command=calendargetter)
my_button2.pack(pady=20)


my_label= tb.Label(root, text="You picked: ")
my_label.pack(pady=20)

root.mainloop()

"""

"""

from tkinter import *
import ttkbootstrap as tb


root = tb.Window(themename=("cyborg"))

#root = Tk()
root.title("TTK BOOTSTRAP")
#root.iconbitmap("images/codemy.ico")
root.geometry("500x350")

def thing():
    pass

my_frame = tb.Frame(root, bootstyle="dark")
my_frame.pack(pady=40)

my_entry = tb.Entry(my_frame ,font=("Helvetica", 18))
my_entry.pack(pady=20,padx=20)

my_button = tb.Button(my_frame, text="Click me", bootstyle="dark",command=thing)
my_button.pack(pady=20,padx=20)

my_label = tb.Label(root,text="hello there",font=("Helvetica",18), bootstyle="inverse light")
my_label.pack(pady=20)

root.mainloop()

"""

"""

from tkinter import *
import ttkbootstrap as tb


root = tb.Window(themename=("superhero"))

#root = Tk()
root.title("TTK BOOTSTRAP")
#root.iconbitmap("images/codemy.ico")
root.geometry("500x350")

def stuff(x):
    my_menu.config(bootstyle=x)
    my_label.config(text =f"You Selected {x}")


my_menu = tb.Menubutton(root,bootstyle="warning",text="things")
my_menu.pack(pady=50)

inside_menu = tb.Menu(my_menu)

item_var = StringVar()
for x in ["primary","secondary","danger","info","outline primary","outline swimmer"]:
    inside_menu.add_radiobutton(label=x, variable=item_var,command=lambda x=x:stuff(x))

my_menu["menu"] = inside_menu

my_label = tb.Label(root, text="")
my_label.pack(pady=40)

root.mainloop()

"""

"""  #frames and labels

from tkinter import *
import ttkbootstrap as tb


root = tb.Window(themename=("superhero"))

#root = Tk()
root.title("TTK BOOTSTRAP")
#root.iconbitmap("images/codemy.ico")
root.geometry("500x350")

def thing():
    pass


my_frame =tb.Frame(root, bootstyle="light")
my_frame.pack(pady=40)

my_entry = tb.Entry(my_frame, font=("Helvetica",18))
my_entry.pack(pady=20,padx=20)

my_button = tb.Button(my_frame,text="click me",bootstyle="dark,",command=thing)
my_button.pack(pady=20,padx=20)

my_label = tb.Label(root ,text="hello there",font=("Helvetica",18),bootstyle="light inverse") 
my_label.pack(pady=20)

root.mainloop()      

"""

"""# widgets

from tkinter import *
import ttkbootstrap as tb


root = tb.Window(themename=("superhero"))

#root = Tk()
root.title("TTK BOOTSTRAP")
#root.iconbitmap("images/codemy.ico")
root.geometry("500x550")

global counter
counter=5

def clicker():
    global counter
    if counter <= 100:
        my_meter.configure(amountused=counter)
        counter += 5
        my_button.configure(text=f"click me {my_meter.amountusedvar.get()}")


def up():
    my_meter.step(10)

def down():
    my_meter.step(-10)


my_meter = tb.Meter(root,
                     bootstyle="danger",
                     subtext="meter",
                     interactive=True,stripethickness=10,
                     padding=20,
                     amountused=0,
                     subtextstyle="light",
                     amounttotal=100)#textright=% can be used here so can meter type
my_meter.pack(pady=50)

my_button = tb.Button(root,text="click 5",command=clicker)
my_button.pack(pady=20)


my_button2 = tb.Button(root,text="step up",command=up)
my_button2.pack(pady=20)


my_button3 = tb.Button(root,text="step down",command=down)
my_button3.pack(pady=20)

root.mainloop()      


"""

""" #textbox notebook thing

from tkinter import *
import ttkbootstrap as tb


root = tb.Window(themename=("superhero"))

#root = Tk()
root.title("TTK BOOTSTRAP")
#root.iconbitmap("images/codemy.ico")
root.geometry("500x550")

my_notebook = tb.Notebook(root,bootstyle="dark")
my_notebook.pack(pady=20)

tab1 = tb.Frame(my_notebook)
tab2 = tb.Frame(my_notebook)

my_label = tb.Label(tab1, text="my label",font=("Hevetica",18))
my_label.pack(pady=20)

my_text = Text(tab1,width=70,height=10)
my_text.pack(pady=10,padx=10)

my_button = tb.Button(tab1,text="click", bootstyle="danger outline")
my_button.pack(pady=20)

my_label2 = tb.Label(tab2, text="my label",font=("Hevetica",18))
my_label2.pack(pady=20)

my_notebook.add(tab1,text="tab1")
my_notebook.add(tab2,text="tab2")

root.mainloop()      


"""
