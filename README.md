# TwitchLink - Mac
TwitchLink of MacOS version.


# Original Project
- [HomePage](https://twitchlink.github.io)
- [Source Code](https://github.com/devhotteok/TwitchLink)


# Requirements & Download

- **MacOS** Required
- Installer (.dmg) is prepareing. thank you for your patience


# Changes from Windows version

#### Overall Feature/Function changes
***
##### Disabled -

- NewDownloader
    - This function will be available at ***Next version***
  
- Auto Update
    - Reason : Auto Update is based on **Windows OS**  




#### [TwitchLink.py](https://github.com/Leatherback-Azi/TwitchLink-MacOS/blob/main/TwitchLink.py)
***
##### Function -

- **checkStatus** in class **TwitchLink**

    - Auto Update Check disabled.

- **NewDownlaoder** has been **disabled**

    - Reason : Function **os.startfile dosen't support MacOS.**
    - This function will be available at **next version**.
   
   
#### [TwitchLinkConfig.py](https://github.com/Leatherback-Azi/TwitchLink-MacOS/blob/main/TwitchLinkConfig.py) 
***
##### Value -

* **All of Directory** has been Changed compatible as **MacOS**

#### [TwitchLink-MacOS/Auth/](https://github.com/Leatherback-Azi/TwitchLink-MacOS/tree/main/Auth)
***
##### Function -

- Code below has been **disabled** in **both Engines**
    - Reason : Not compatible with MacOS
    <pre><code>  startupinfo = subprocess.STARTUPINFO()
    startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW    </code></pre>


#### [Auth/TwitchUserAuthWebDriverLoader.py](https://github.com/Leatherback-Azi/TwitchLink-MacOS/blob/main/Auth/TwitchUserAuthWebDriverLoader.py)
***
##### Top of code -

- Code below has been **disabled**
    - Reason : Dosen't need to MacOS
    <pre><code>  from webdriver_manager.microsoft import EdgeChromiumDriverManager
    from Auth.TwitchUserAuthSeleniumService import Service

    webdriver.chrome.service.service.Service.start = Service.start
    webdriver.edge.service.service.Service.start = Service.start  </code></pre>
    
    
#### Auth/TwitchUserAuthSeleniumService.py
***
##### DELETED!

- Reason : Not Compatible with MacOS, and dosen't need to Special setup with Selenium


