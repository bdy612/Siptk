# Intro

Hi there, this is SIPTK if you want to know more about SIPTK go to https://github.com/bdy612/Siptk/blob/main/README.md

# Starter

To start the program, just choose which Type of SIPTK do you want to choose in the latest version (0.0.2) there are 2 ways: siptk1 and siptk2. Siptk1 is made by Ahmed Islam and Siptk2 is made by Abdelrahman Ahmed

If you want siptk1 just write:
import siptk
window = siptk.siptk1()
window.label("hi how are you")
enter = window.entry()
window.button("Did you dare to click me!?", lambda: window.label(get_entry_value(enter)))

This is just a bunch of code for a simple window

If you want siptk2 just write:
import siptk as tk
window = tk.siptk2(title="SPSL", width=500, height=400)

text1 = tk.Label(window, text="Hi this is SPSL")

window.run()

NOTE: in siptk2, you can't write "from siptk import siptk2" because there are more classes for the components
