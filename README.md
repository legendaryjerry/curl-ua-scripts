# curl-ua-scripts
Present SysAdmin Commands via cURL

This project will use Apache to detect the user-agent of a request and redirect cURL requests to a directory structure that contains common administrative commands and scripts. The commands and scripts can then be piped to a shell to be executed. 

Usage
$ curl -s example.com/[***FILENAME***]|/bin/bash

Example
$ curl -s example.com/sysinfo|/bin/bash

Disclaimer
Review commands before you run them by running curl -s example.com/[***FILENAME***]

Cron Job (optional)
This is used to sync the curl-ua-scripts git project to local a repository that is linked or periodically synced to the public web directory. 
15 * * * * /root/scripts/gitsync > /root/logs/gitsync.log 2>&1
