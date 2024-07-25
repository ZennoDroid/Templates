## Hamster Kombat Bot Setup Instructions.  
The Hamster Kombat bot **automates the coins collection** in the **Hamster Kombat** app and **works using the ZennoDroid Lite/Pro** program. The bot has input settings for building a flexible work scheme using taps and some other features.  

**1.Download and install the demo version of** [**ZennoDroid**](https://drive.google.com/drive/folders/1sHjuft2GyKsk0dwlG0XSL51Hdp8bQAM3)  

**2.Add the bot to ZennoDroid**    
- Add the bot to ZennoDroid.  
- Configure input parameters:  
    - specify the path to the Telegram `.apk` file. The bot will install Telegram on the emulator if it is missing, and will offer to manually set up an account using a phone number and verification code.  

All other bot settings can be left unchanged, as the optimal settings are already set.  

**3. Emulator setup**  
&nbsp; Specify the name of the MEmu emulator you will work with. 
&nbsp; The emulator should be created beforehand in the MEmu device manager.  

**4. Extra options**  
- Optimal settings are preset. You can leave them unchanged.  
- The bot can automatically monitor the energy level and resume taps if the energy has risen above the value specified in the input settings (default 500).  
The bot uses an adaptive dynamic pause, instead of the previously used fixed pause.   
- Included improvements to speed up coin collection:  
    - **Daily rewards:** over 6 million coins in 10 days.  
    - **Boost/Full Energy:** regular enhancement of collection efficiency. 

![Входные параметры](https://i.ibb.co/CtsyDKz/Humster-ZD.jpg)  

### Recommendations  
- Use the emulator with Android 9.0 x64 for best performance. Android 7.1 x64 with an updated WebView component is also supported.  
- We recommend that you manually launch the emulator and update the Chrome browser (the WebView component will be updated along with it) before using the bot for the correct operation of mini-applications in Telegram. How to update the Chrome browser to the latest version is described [**here**](https://zenno.club/discussion/threads/ne-zagruzhajutsja-boty-v-telegramm.120040/#post-798558).  
- Embed the updated version of Chrome into the MEmu base image, so you don't have to update Chrome on each emulator separately. For more information [please contact us](https://helpdesk.zennolab.com/en-us/conversation/new).  
### Fixes  
&nbsp; ✚ Replaced “**Search by picture**” with a more reliable method of selecting Hamster in the Telegram app contact list, as 'Search by picture' gave frequent misses. It was possible to optimize, but it was faster to use another option, which is obviously more reliable and does not require tweaks and experiments.  

&nbsp; In the new method, you activate “**Search by contacts**” and enter Hamster Kombat there, the desired account appears in the first line, and you touch it using the usual reliable method. The big plus of this method is that there is no need to swipe, which also adds stability to the work of the bot.  

&nbsp; ✚ Fixed a critical bug in one of the important functions (“**Daily Reward**”). Fixed an action that can give a critical failure - analyzing the need to pick up the "Daily Reward".  

&nbsp; ✚ In the “**Set number of taps**” mode now does not auto-add a project attempt when the project is interrupted and stopped, this is important for correct work on schedule.  

&nbsp; ✚ Implemented the ability to enter percentages rather than quantities in the input settings field: “**Resume taps when Energy level is reached**”. This will also auto randomize the percent value +-25%, as it happens when applying for a regular number in this field. That is, 
using percentages will adaptively adjust the maximum threshold for when to start tapping.   

&nbsp; ✚ Fixed failed generation of upper random limit of tracked energy level.  

&nbsp; ✚ Fixed bot freezing in some rare cases.  

&nbsp; ✚ Added touch to the button to accept a bonus from the exchange or to the level up button during the 'Work Interval' polling interval.  

&nbsp; ✚ Added possibility to enter 'Daily Cipher' (by Morse code) when restarting the bot. The code should be written in the text file daylycode.txt next to the bot file, in one line, separating separate character codes with a space.   

&nbsp; &nbsp; For example, the word **GAS**:  

&nbsp; &nbsp; &nbsp; &nbsp; 1. letter G: `— — •`  
&nbsp; &nbsp; &nbsp; &nbsp; 2. letter A: `• —`  
&nbsp; &nbsp; &nbsp; &nbsp; 3. letter S: `• • •`  

&nbsp; &nbsp; It should be written like this: `--. .- ...`  
&nbsp; &nbsp; (`--.<space>.-<space>...`)  

&nbsp; ✚ Added calculation of project run-time in hours and minutes.  

&nbsp; ✚ Added search phrase setting and contact number for selection in the input settings. It happens that there are a lot of additional contacts in Telegram contacts and they become the first place, so the bot enters the wrong contact and cannot launch the application.

