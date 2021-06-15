# TwitchLink - Mac
TwitchLink of MacOS version.


# Original Project
- [HomePage](https://twitchlink.github.io)
- [Source Code](https://github.com/devhotteok/TwitchLink)


# Requirements & Download

- **[OS X](https://en.wikipedia.org/wiki/MacOS)** or Higher (macOS)
- **[Chrome](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwjQhO3jtp_vAhVSHaYKHVL2CfkQFjAAegQIBBAE&url=https%3A%2F%2Fwww.google.com%2Fintl%2Fko%2Fchrome%2F&usg=AOvVaw13CftYisc_84G1d2VQFf-w)** Web browser
- Installer (.dmg) is prepareing. thank you for your patience


# Changes from Windows version

#### Overall Feature/Function changes
***
##### Disabled -

- NewDownloader
    - This function will be available at ***Next version***
  
- Auto Update
    - Reason : Auto Update is based on **Windows OS**  




#### [/TwitchLink.py](https://github.com/Leatherback-Azi/TwitchLink-MacOS/blob/main/TwitchLink.py)
***
##### Function -

- **[checkStatus, setupmenubar](https://github.com/Leatherback-Azi/TwitchLink-MacOS/blob/main/TwitchLink.py#L78)** in class **TwitchLink**

    - [Auto Update Check](https://github.com/Leatherback-Azi/TwitchLink-MacOS/blob/main/TwitchLink.py#L105) disabled.

- **NewDownlaoder** has been **disabled**

    - Reason : Function **os.startfile dosen't support MacOS.**
    - This function will be available at **next version**.
    
    
#### [/TwitchLinkUi.py](https://github.com/Leatherback-Azi/TwitchLink-MacOS/blob/main/TwitchLinkUi.py)
***
##### UISize -

* UISize has been changed
    * Code : 'windowsize' in [VideoList](https://github.com/Leatherback-Azi/TwitchLink-MacOS/blob/main/TwitchLinkUi.py#L605) Class
    * Reason : Existing value is not compatible with MacOS
   
   
#### [/TwitchLinkConfig.py](https://github.com/Leatherback-Azi/TwitchLink-MacOS/blob/main/TwitchLinkConfig.py) 
***
##### Value -

* **All of Directory** has been Changed compatible with **MacOS**

#### [/Auth/](https://github.com/Leatherback-Azi/TwitchLink-MacOS/tree/main/Auth)
***
##### Function -

- Code below has been **disabled** in **both Engines**
    - Reason : Not compatible with MacOS
    <pre><code>  startupinfo = subprocess.STARTUPINFO()
    startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW    </code></pre>


#### [/Auth/TwitchUserAuthWebDriverLoader.py](https://github.com/Leatherback-Azi/TwitchLink-MacOS/blob/main/Auth/TwitchUserAuthWebDriverLoader.py)
***
##### Top of code -

- Code below has been **disabled**
    - Reason : Dosen't need to MacOS
    <pre><code>  from webdriver_manager.microsoft import EdgeChromiumDriverManager
    from Auth.TwitchUserAuthSeleniumService import Service

    webdriver.chrome.service.service.Service.start = Service.start
    webdriver.edge.service.service.Service.start = Service.start  </code></pre>
    
    
#### [/resources/ui/](https://github.com/Leatherback-Azi/TwitchLink-MacOS/tree/main/resources/ui)
***
##### UI changes -

- File below has been changed as compatible with MacOS
    - search.ui, videoList.ui, downloadMenu.ui, search.ui, videoList.ui, videoFrame.ui


#### [/resources/dependencies/ffmpeg](https://github.com/Leatherback-Azi/TwitchLink-MacOS/blob/main/resources/dependencies/ffmpeg)
***
##### File changes -
- "ffmpeg.exe" has been changed to "ffmpeg"(Unix Excutable File)
    - Reason : MacOS dosen't Support **.exe** formet.
    
    
#### Auth/TwitchUserAuthSeleniumService.py
***
##### DELETED!

- Reason : Not Compatible with MacOS, and dosen't need to Special setup with Selenium


