# RunAsDate-for-MacOS
A "Run as Date" launcher is a tool that allows you to run an application on a specific date and time, rather than the current date and time. This can be useful for testing software that has expiration dates, or for running older versions of applications that are no longer supported on the current operating system.

Until recently, this type of tool was not available for macOS. However, I have found a way to create a "Run as Date" launcher for macOS.

# The solution
When trying to solve the "Run as Date" problem on macOS, I first researched existing solutions and found that there were no readily available tools for this specific task. However, I knew that it was possible to change the system date and time using Terminal commands, so I began experimenting with different command line utilities to see if I could find a way to automate the process.

After some experimentation, I discovered that I could use a combination of the "date" command and the "open" command to change the date and launch an application. I created a simple shell script that included these commands and was able to successfully run an application on a specific date.

Next, I wanted to make this process more user-friendly and accessible to others, so I decided to convert the shell script into an Apple Shortcut. I used the "Run Script" action in the Shortcuts app to run the shell script, and added additional actions to make the shortcut more functional and intuitive to use.

Overall, it was a process of experimentation and problem solving, but I was able to find a way to automate the "Run as Date" process using Terminal and shell script, and then convert it into an Apple Shortcut for easy use.

# Instructions ( What you need to do ? )
To use the Apple Shortcut, follow these steps:

 1. Download the shortcut from the github repository.
 2. Double click and add the shortcut to your library.
 
    <img width="427" alt="Screenshot 2023-01-24 at 10 42 32 AM" src="https://user-images.githubusercontent.com/71588718/214216981-c59d1624-3508-4378-be32-3eaf514620a8.png">
    
 3. In the app double click the shortcut (not the play button).
 5. In the script you can change the specific date . The format to the date is :  MMDDHHmmYY .  where "M" is for month and "m" is for minute.
 
    <img width="606" alt="Screenshot 2023-01-24 at 10 45 50 AM" src="https://user-images.githubusercontent.com/71588718/214217148-ab15b0cd-573d-4ae7-ac0f-2a0d73e6af36.png">
    
 6. You can change the application buy replacing the /Applications/Infuse.app with your application's location.
 7. If you face any issue while launching ( especially if the launch is slow you can try and change the " sleep 6 " code , here 6 stands for 6seconds of delay befor the date is reverted back to current date .
 8. Give a name to the shortcut, and tap "Done" to save it.
 9. You can now run this shortcut by tapping on it in the Shortcuts app or by using Siri.

You can also customize the shortcut by adding more actions, for example you can add an action to ask for the desired date and application every time you run the shortcut.

It's important to remember that the script is running on the user level and it changes the system date.






