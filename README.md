# saladfork-mainsail-theme
SSH console
Your console should appear similar to this.

putty_normal_view

Console Commands
Paste the following code into your console.

    cd ~/
    git clone https://github.com/shawnchr/saladfork-mainsail-theme.git
    bash ~/saladfork-mainsail-theme/install.sh

After pasting them into the console, it should resemble this.

<img width="1256" height="75" alt="image" src="https://github.com/user-attachments/assets/73989e8a-3e1f-4a35-b190-16042e36c24a" />


The input field still shows a command we have to run, press ENTER on your keyboard to run the command.

Once executed, your console should display the message ‘Theme has been installed, have fun!’ indicating that this step is now complete.

<img width="934" height="280" alt="image" src="https://github.com/user-attachments/assets/eebcb7bf-2bbf-4d41-a09d-fa776d1ea0a9" />


Machine Settings
For the next step of the instructions, you will be using your web client.

To begin, open the web client of your printer. On the left-hand side of the interface, locate the menu and click on ‘Machine’.

<img width="220" height="337" alt="image" src="https://github.com/user-attachments/assets/df9c480b-a84e-4b04-b709-9072fc41f138" />

Config Files
Locate the file ‘moonraker.conf’ and click on it.

<img width="814" height="501" alt="image" src="https://github.com/user-attachments/assets/c297ae6d-a06d-4c40-b2e4-4c05f59b2d6a" />

Adding Update Script
Scroll down until you find the text [update_manager].

If you see an additional line that reads “enable_auto_refresh: True”, do not remove it. Simply proceed to the next line. Note that this line may not be present for all users.

update_manager

Insert the following code:

    [update_manager client SaladForkTheme]
    type: git_repo
    path: ~/saladfork-mainsail-theme
    origin: https://github.com/shawnchr/saladfork-mainsail-theme.git
    install_script: install.sh
    is_system_service: False

Your configuration should now resemble the following:

pasted_update_manager

Save & Restart
Click on the Save & Restart button.

save_restart

Restart Moonraker
If a notification appears asking you to try again, click on it to proceed.

try_again

Refresh your browser
Refresh your browser to check if the ZeroG theme is now visible.

refresh

Update manager
On the right-hand side, you will see the Update Manager. You should now notice that ZeroGTheme has been added. This will enable you to easily obtain the latest updates as they become available for the ZeroG Mainsail Theme.

update_manager

Screenshot
You now have a fresh new theme to enjoy. With its sleek new design, your ZeroG experience just got a whole lot better. So sit back and enjoy the ride - the view has never looked better!
