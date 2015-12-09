# redShift
instructions to make computer redshifted using crontab

open a terminal
enter command: crontab -e
if prompted select an editor (best is #2 the nano editor in my opinion)
Go to the bottom of the file and add these lines:

SHELL=/bin/sh
PATH=/usr/local/sbin:/usr/local/bin:/sbin:/bin:/usr/sbin:/usr/bin
0-59/5 20-23 * * * export DISPLAY=:0.0 && /usr/bin/xgamma -rgamma 1.5 && /usr/b$

The entire file should look similar to this:

  GNU nano 2.2.6                                                    File: /tmp/crontab.sCvlzY/crontab                                                                                                              

# Edit this file to introduce tasks to be run by cron.
#
# Each task to run has to be defined through a single line
# indicating with different fields when the task will be run
# and what command to run for the task
#
# To define the time you can provide concrete values for
# minute (m), hour (h), day of month (dom), month (mon),
# and day of week (dow) or use '*' in these fields (for 'any').#
# Notice that tasks will be started based on the cron's system
# daemon's notion of time and timezones.
#
# Output of the crontab jobs (including errors) is sent through
# email to the user the crontab file belongs to (unless redirected).
#
# For example, you can run a backup of all your user accounts
# at 5 a.m every week with:
# 0 5 * * 1 tar -zcf /var/backups/home.tgz /home/
#
# For more information see the manual pages of crontab(5) and cron(8)
#
# m h  dom mon dow   command
SHELL=/bin/sh
PATH=/usr/local/sbin:/usr/local/bin:/sbin:/bin:/usr/sbin:/usr/bin
0-59/5 20-23 * * * export DISPLAY=:0.0 && /usr/bin/xgamma -rgamma 1.5 && /usr/bin/xgamma -ggamma .5 && /usr/bin/xgamma -bgamma .1

