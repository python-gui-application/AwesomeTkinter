AwesomeTkinter offers some new and pretty tkinter widgets

example widgets:  
radial progressbar, scrollable frames, 3d buttons, 3d frames, and more.

also, you can use a lot of useful functions that can manipulate images,
e.g. to create tkinter PhotoImage from a file but want to change its
size and color you can `img = atk.create_image(fp='path to my image
file', color='red', size=100)`

# Screenshots:
![progressbar](https://user-images.githubusercontent.com/37757246/93201974-382be080-f752-11ea-8bc1-183f9bcb6b58.png)
--------------------------------------------------------------------------------------------------------------------

# Applications Made with AwesomeTkinter:
![PyIDM](https://user-images.githubusercontent.com/58998813/92564079-e4fcee00-f278-11ea-83e1-9a272bc06b0f.png)

# Installation:
`python3 pip install awesometkinter`

for quick test:
```
import awesometkinter as atk
atk.main()
```

or from terminal:
```
python3 -m awesometkinter
or just
awesometkinter
```
this will display a test window

# Requirements:
- minimum python version 3.6
- tkinter
- pillow

# Example:
```
import tkinter as tk
import awesometkinter as atk

root = tk.Tk()
root.config(background=DEFAULT_COLOR)

f1 = atk.Frame3d(root)
f1.pack(side='left', expand=True, fill='both', padx=3, pady=3)

bar = atk.RadialProgressbar3d(f1, fg='cyan', size=120)
bar.pack(padx=20, pady=20)
bar.start()

atk.Button3d(f1, text='3D Button').pack(pady=10)

f2 = atk.Frame3d(root)
f2.pack(side='left', expand=True, fill='both', padx=3, pady=3)

bar = atk.RadialProgressbar(f2, fg='green')
bar.pack(padx=30, pady=30)
bar.start()

btn = atk.Button3d(f2, text='Pressed Button')
btn.pack(pady=10)

root.mainloop()
```

# Documentations:
TBA

---
# Author:
Mahmoud Elshahat  
2020
