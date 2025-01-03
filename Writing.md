# Intro

Hi there, this is SIPTK if you want to know more about SIPTK go to (README.md)[https://github.com/bdy612/Siptk/blob/main/README.md]

# Starter

To start the program, just choose which Type of SIPTK do you want to choose in the latest version (0.0.2) there are 2 ways: siptk1 and siptk2. Siptk1 is made by Ahmed Islam and Siptk2 is made by Abdelrahman Ahmed

## Siptk1

If you want siptk1 just write:

> import siptk
> window = siptk.siptk1()
> window.label("hi how are you")
> enter = window.entry()
> window.button("Did you dare to click me!?", lambda: window.label(get_entry_value(enter)))

This is just a bunch of code for a simple window

## Siptk2

If you want siptk2 just write:

> import siptk as tk
> il = 0
> window = tk.siptk2(title="SPSL", width=500, height=400)
> text1 = tk.Label(window, text="Hi this is SPSL")
> def change():
>  root = TopLevel(window, title="Sorry error")
>  text2 = tk.Label(root, text="Hi silly")
> if il == 0:
>    text1.config("Silly Hi this is SPSL")
>   il = 1
>  elif il == 1:
>    text1.config("Hi this is SPSL")
>    il = 0
>  else:
>    pass
> button1 = tk.Button(window, text="Click to change", command=change)
> window.run()

## Notes

NOTE: in siptk2, you can't write "from siptk import siptk2" because there are more classes for the components

# Writing

To write code for Siptk let's divide this to 2 parts.
First part will talk about Siptk1
Second part will talk about Siptk2

## Part 1

To start, import Siptk and initialize the app

> import siptk as tk
> window = tk.siptk1(title="Welcome to Siptk", size="1000x500")

NOTE: in the window, there aren't any more things I can put in it like "Resizeable" isn't in Siptk1

Next, Let's add components

> text1 = window.label("Siptk", bg="Green", fg="Blue", width=100, height=100)
> button1 = window.button("Click to print", button1, bg="Green", fg="Blue", width=100, height=100)
> entry1 = window.entry(default_text="your EMAIL", bg="Green", fg="Blue", width=100, height=100)
> check1 = window.checkbox("Hi there", bg="Green", fg="Blue", width=100, height=100)
> scale1 = window.scale(from_=0, to=20, bg="Green", fg="Blue", width=100, height=100)   NOTE: the scale will have the orient=tk.HORIZONTAL
> canvas1 = window.canvas(100, 100, bg="Green")
> image1 = window.image(icon.jpg, height=100, width=100)
> listy = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
> combobox1 = window.cobox(listy)
> list_box1 = window.list_box(listy)
> menu1 = window.menu()
> menu_item1-1 = window.menu_item(menu1, listy[5], menuitem)
> menu_sparator = window.separator(menu1)
> window.message_box("Message from Siptk", "Hi silly, enough talking together")
> quest = window.question_box("Hi there", "Are you Ahmed Islam")
> window.warning_box("Hi there", "There is a warning for a rocket on your head")
> window.error_box("ERROR", "AN ERROR!!!!")
> frame = window.frame(bg="Green", fg="Red")
> window.run()

Now, we have too many components, we want to make it more interactive, continue our code to see
NOTE: Our code which we will make now will be before the components

Now, let's make it more interactive

> def button1():
>   text_for_entry = window.get_entry_value(entry1)
>   print(text_for_entry)
>   checkbox_info = window.get_checkbox_value(check1)
>   print(checkbox_info)
>   selection = get_list_box_value(list_box1)
>   print(selection)
>
> def menuitem():
>   intvar = window.create_intvar()
>   scale_info = window.scale_value(scale1)
>   value_for_combo = window.combo_box_value(combobox1)
>   print(scale_info)
>   print(value_for_combo)

Like that we have a huge code for Part 1, What could we do in **Part 2**?

## Part 2
