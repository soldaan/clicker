import keyboard , time , pyautogui

work = False

def change():
    global work
    work = not work
keyboard.add_hotkey('`', change)
while True:
    if work:
        pyautogui.leftClick()
        time.sleep(0.1) 
