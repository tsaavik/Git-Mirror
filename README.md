Git-Mirror
==========

Automatically Keeps a directory full of git mirrors up to date with remote
David Mcanulty 2013

Requires: Cron - for updates
          git  - for doing git operations

To start Mirroring a new GIT repo:
   cd /home/yourname/gitmirror/
   git clone --mirror git@github.com:YOURGITNAME/REPONAME

Example cron entry for keeping mirrors up to date once a day:
   23 4 * * * git-mirror ~/gitmirrors/ >>/var/log/git-mirror.log 2>&1
