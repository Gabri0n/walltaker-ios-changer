# walltaker-ios-changer

This IOS shortcut will use the walltaker API to set your Iphones wallpaper. Due to limitations in IOS,
shortcuts cant resonably be setup to periodically run at consistent times without setting automations 
every X amount of time in the shortcuts app, in other words if you wanted to update it every minute 
you would have to manually add an automation to run every minute of the day. 

You can however set the shortcut to run whenever you open specified apps!
This lets you set whichever apps you may use the most so that the shortcut can run whenever you open
your browser, youtube, tiktok etc... While its not optimal this seems to be the best way to set the
wallpaper without forking the cash over for apple to have your app in the store.

## How to Use

To use it simply download the shortcut to your IOS device from below:

[Download Link](https://www.icloud.com/shortcuts/cf59e235d2a745e68daad955e2742605)

Once downloaded it should prompt you for some set up steps such as entering your Walltaker link, selecting
whether to set the Lock Screen, Home Screen, or both, and choosing the wallpaper preset. **NOTE:** You may need
to create a wallpaper preset if the options are greyed out. You can fix this through: 
  **Settings > Wallpaper > and creating a new wallpaper with a photo background**

![Setup Steps Video](/content/gif1.gif)

Once this is done it should allow you to select it. If you need to rerun the setup this can be done through:
  **Shortcuts > Walltaker IOS Switcher > Selecting the (i) icon in the bottom middle > Setup > Customize Shortcut**

Now, from within the shortcuts app, navigate to the automations tab and create a new automation (you can make multiple) targeting your app of choice and then selecting the Walltaker IOS Switcher shortcut as the target.


![Automation Steps Video](/content/gif2.gif)

The first 1-2 times the shortcut is run it may prompt for permissions to A) Use your browser and B) Access your files.
The shortcut requires browser permission to access the walltaker API and retrieve the image information. The shortcut also requires files permission so that it can save
a copy of the e621 URL. The purpose of this is to not set your wallpaper if it hasnt changed, this is to prevent unnececary data usage by redownloading image data whenever the shortcut is run. The shortcut will store this at Downloads/walltaker.txt and use it to check against the URL retrieved from the Walltaker API.
