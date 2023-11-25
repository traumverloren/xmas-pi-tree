# xmas-pi-tree

Simple python script for my led gpio xmas tree

Setup the lights to turn on/off on schedule with cronjob:

Edit the cronjob file by doing `sudo crontab -e` & adding the following:

```bash
@reboot python3 /home/pi/xmas.py

0 7 * * *  python3 /home/pi/xmas.py
0 22 * * * killall -2 python3
```
