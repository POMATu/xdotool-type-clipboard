# xdotool-type-clipboard
This tool types everything from your clipboard to active window. That can be useful to transfer clipboard to guest operating system if you are using virtual machines without guest additions module, and some buggy VNC/RDP connections (and even pasting to UAC cmd.exe which is usually crap when using via RDP).

# Demonstration


# Requirements 
* Linux host
* Window to past to
* You need to setup delay before key invocation so you will be able to make your window active
* Dependencies:
```sudo apt install xclip xdotool```

# How to use
1. Copy text to clipboard
2. Launch:
```
bash xdotool-type-clipboard 3
``` 
That means that script will wait for 3 seconds and then type everything from keyboard to active window. 3-5 seconds is usually enough to focus on needed window
