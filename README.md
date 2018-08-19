# Gist-watcher
Creates a cron job to monitor a Gist feed, on new posts an arbatory command is exicuted.

This bash script, when run, asks for a Github username, the username is checked using the Github API for validity, on error it asks again.
The second question is the frequency the cron job is to run at, if the answer contains a "d", as in "daily" the cron job will be run every 24 hours, else it is run every hour.

The created cron jobs are made in /etc/cron.daily or /etc/cron.hourly

