# udemy-downloader
Udemy purchased course downloader with various quality

## Intialization of credentials
* Just run `udemy.exe` It will show a javascript code to execute and ask to paste output as well. 
* Copy the code and keep. 
* Now login in to your udemy account [Udemy](https://www.udemy.com/). 
* After successful login, run the copied command in browser console window. If you don't know to open console window then refer [this](https://stackoverflow.com/questions/66420/how-do-you-launch-the-javascript-debugger-in-google-chrome)
* It will print some output (logged in session cookies in base64 encoded format). 
* Copy the output and paste in command prompt and press enter.
* You can see one properties file created in the following location `%APPDATA%\udemy-downloader\udemy.properties`

## How to use
usage: `udemy.exe [-h] [-u URL] [-c CLEAR] [-q QUALITY]`

optional arguments:
  -h, --help            show this help message and exit
  -u URL, --url URL     udemy course url
  -c CLEAR, --clear CLEAR
                        clear saved udemy credentials details
  -q QUALITY, --quality QUALITY
                        specify video quality as high/medium/low/verylow.
                        default is high

example: `udemy.exe -u https://www.udemy.com/aws-concepts/ -q medium`

## How to clear saved credentials
`udemy.exe -c CLEAR`
To verify, check `%APPDATA%\udemy-downloader\udemy.properties` location

## Known bugs
* Not handled when internet connection is not there
* Tested for few courses, so for some courses it can behave weird (I don't know :grin:)
* If anything you finds, please feel free to create an Issue in github

## Raise query
Feel free to raise issues in github. If you want to get in touch ping me in [Telegram](https://t.me/thegr8uk)