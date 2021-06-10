# Overview
[![License](https://img.shields.io/badge/License-View%20License-orange)](http://www.glocomp.com/)

SecureKi will integrate with Cisco Duo and Webex Team.

- Cisco Duo to provide multifactor authentication
- Webex Team space to receive and display event notifications.

# Installation

OS System:
```
$ pip install duo-client
```
# Description
**check_mobile_ext_auth.sh**  - To send Cisco Duo Push authentication to mobile device

**check_web_otp.sh**          - To check Cisco Duo Passcode Authentication

**syslog.sh**                 - To detect system logs and events and call curlsend.py to send the notification

**curlsend.py**               - To send event notification or policy violations to Webex Teams


## Usage
Upload the scripts to OS. Edit the script to include Cisco Duo API Host, IKEY and SKEY.

IKEY=""

SKEY=""

HOST=""


To run the query, execute a command like the following:

```
$ ./check_mobile_ext_auth.sh <username>
$ ./check_web_otp.sh <username> <passcode>
$ python curlsend.py
```

## Contributing
GR4-Glocomp
