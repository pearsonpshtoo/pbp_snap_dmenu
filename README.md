# pbp_snap_dmenu
guide to create a script that launches an installed snap application in dmenu on a pinebook pro running manjaro 20 with i3 as the tiling manager

1) create script that launches snap application in home dir or other location to remember
  ex) "vim chromium_snap.sh" & type "snap run chromium" then save
2) make script executable
  ex) "chmod +x chromium_snap.sh"
3) make link to script in /bin/ folder, where dmenu checks for applications
  ex) "sudo ln /home/user/chromium_snap.sh /bin/chromium_snap" replacing "home/user/" if the script is not in home dir


you should then be able to search dmenu in i3 by pressing the modifier key and "d" and typing "chromium_snap" or whatever you named the link
