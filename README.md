# redShift
instructions to make computer redshifted using crontab

open a terminal
enter command: crontab -e
if prompted select an editor (best is #2 the nano editor in my opinion)
Go to the bottom of the file and add these lines:

SHELL=/bin/sh
PATH=/usr/local/sbin:/usr/local/bin:/sbin:/bin:/usr/sbin:/usr/bin
0-59/5 20-23 * * * export DISPLAY=:0.0 && /usr/bin/xgamma -rgamma 1.5 && /usr/b$

The entire file should look like the crontab file in this git repo
