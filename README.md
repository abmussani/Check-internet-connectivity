Check internet connectivity
===========================

<b>Problem</b>

To check internet is working or not, everyone has to first open the browser and then visit <a href="http://www.google.com">Google</a>. If you see google homepage then you are connected otherwise not. I tried to developed a better solution that computer itself will visit google.com and will tell you either connection is down or not.


<b>Logic</b>

It is a on going process. First computer will send a curl request to Google. If http response is successfull then script will wait 120 seconds before executing next iteration. It http response is not successfull then it will wait for 5 seconds before executing next iteration.

This script also produces voice for distant users (how can hear the voice, like people sitting at another corner of room). On connectivity, "Internet Connection" words will be speak by the system and if connection is down then "Internet Disconnected" will be pronounce by the system.


<b>Technology Required</b>

Mac OSX 10.9, 
AppleScript

<b>How to run applescript file</b>

1- Rename file "internet_connectivity_script.applescript" to "internet_connectivity_script.scpt". I have done this to do version controlling on applescript file.<br/>
2- open Terminal (Application / Utility).<br/>
3- In terminal, Navigate to directory where your script file is saved.<br/>
4- Write command "osascript internet_connectivity_script.scpt"<br/>
