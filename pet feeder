from microbit import *

shakes = 0

display.show(Image.YES)
sleep(1000)
display.clear()


while True:

    if accelerometer.was_gesture("shake"):
        shakes += 1
        display.show(shakes)
        sleep(500)
        pin1.write_analog(35)
        sleep(2000)
        pin1.write_analog(80)
        sleep(2000)
    elif button_a.is_pressed():
        display.show(Image.HAPPY)
        sleep(1000)
        display.clear()
        pin1.write_analog(35)
        sleep(2000)
    elif button_b.is_pressed():
        pin1.write_analog(80)
        sleep(2000)
