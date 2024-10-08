# CyberVT-Sep22-Demo

This is the activity for Tuesday, September 24. Please download the file from the main directory but **DO NOT LOOK IN THE FOLDER** if you don't want the answer to be spoiled for you. This is designed to work on an Ubuntu Server image, so some of the challenges might not work if you use a different OS. Good luck!

# Instructions to get started

1. Download the setup script with this command:

    - wget https://raw.githubusercontent.com/bbaum11/CyberVT-Sep24-Demo/refs/heads/main/SetupScript.sh

- If you are using VMWare, you can pase by clicking 'Edit -> Paste' at the top of the window.
- If you are using VirtualBox, enable the shared clipboard with 'Machine -> Shared Clipboard' and set it to Bidirectional.
- If for some reason the Virtualization software is being weird, you're just going to have to type out the link instead.

**I highly reccommend creating a snapshot of your virtual machine before starting this so that you can revert it, since this messes with some system files.**
- VMWare: The clock button with the plus at the top of the window
- Virtualbox: 'Machine -> Take Snaphot'

2. Give execute permissions to the downloaded file and run it with sudo
    - chmod +x SetupScript.sh
    - sudo ./SetupScript.sh

# What to do
This script sets up some malicious activity on your system. It is your job to find the malicious activity and the flags for each thing. The recommended software to use is **rkhunter**. Do some research into how to set up and use rkhunter.

# Helpful hints
- Although the console will show warnings, looking at the logs will provide specific information about each warning found.
    - Look into command line text editors like nano/vim that have search functionality 
- Typing '| less -R' at the end of the search command allows you to scroll back in the terminal
  - The -R preserves the color
  - Using the --sk option for the rkhunter scan allows the scan to run without needing to press <ENTER>
  - Press q to exit this
  - More details will be in the log file
- Please read the comments on the files you find
- Helpful commands
    - ps -aux
    - su <user>
    - cat
    - vim/nano
    - grep
    - ls -a
    - ls -l
- I wonder what suspicious users keep at home...
