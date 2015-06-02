# curl-ua-scripts
Present Common Commands via cURL

This project will use Apache to detect the user-agent of a request and redirect cURL requests to a directory structure that contains common administrative commands and scripts. The commands and scripts can then be piped to a shell to be executed. 

Usage
$ curl -s example.com/[***FILENAME***]|/bin/bash

Example
$ curl -s example.com/sysinfo|/bin/bash

Disclaimer
Review commands before you run them by running curl -s example.com/[***FILENAME***]
