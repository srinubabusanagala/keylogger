Step 1:      Initialize Libraries and Modules 
              •	Import the pynput library to capture keyboard events. 
Step 2:       Define Event Handlers 
              •	Define on_press function to handle and log key press events. 
              •	Define on_release function to handle key release events and stop the listener 
                if the Esc key is pressed. 
Step 3:       Setup and Start Listener 
              •	Create an instance of keyboard.Listener. 
              •	Set the on_press and on_release functions as callbacks for the listener. 
              •	Start the listener to begin capturing keystrokes. 
Step 4:         Log Keystrokes 
              •	In the on_press function, write the captured keystrokes to a log file 
              (keylog.txt). 
              •	Ensure both printable characters and special keys are logged appropriately. 
Step 5:       Stop Listener 
                •	In the on_release function, return False if the Esc key is pressed to stop the 
                  listener
 
