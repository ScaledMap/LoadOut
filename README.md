# LoadOut
LoadOut is a Bookmark manager I've been working on to help manage and organize my bookmarks. It's a Pywebview application built on flask. You can run it as a server or as a webview.  It allows you to import your bookmarks from firefox and create categories to interact with those bookmarks. It would also probably be useful for situations where you want to avoid messing with the keyboard. There was a time where i was using opera because speeddial was useful. I'd kind of like it to be a more flexible alternative to something like opera or speedial. Still kind of a work in progress. I'll probably upload the python script in a bit and a list of packages(requirments.txt) if the exe is too much for ya. Kind of just pick at it when i get bored. Add stuff I think is cool. It could use some optimization. Runs well enough though. My advice would be to run it as a server. You can set it up to boot at startup and set it as the load in page like how pocket would usually load in. An alternative idea would be to change the icon and run it as a server. Would open firefox but on the servers homepage. In the photos section, the desktop is cinnamon. Figure people might wonder about that. 

There are a lot of things I could probably do with this application in the future. More customization would be nice. More default filters. I was thinking about trying to add rss.

----------------------------------------
about
-----------------------------------------
edit may13:Added a default background image. You can switch it back to colors as the default backtround in the customize.ini file. Set the background-image/image to None. Without quotes. You can also change the background image this way. Fixed a but where order wasn't working when loaded from the cardview. Added a notetaking webapp to the project. YOu can create notes based on category in the cardview section. Will open reddit links with a random reddit instance(still need to clean up a bit). It's the same button as convert youtube to invidious as of now.

The linux application has been updated. Added a few settings. atomatically sorts out images. Added navigation options if you want to open up a url inside a webview. Sorts out youtube channels by default. You can see the most recent videos on bookmarked youtube channels. Added an option to open youtube links in a random invidious instance. Added a search bar to search through all your bookmarks. There is a cardview section which is an alternative to using the dropdown. You can choose what bookmarks open when the application is loaded. Bunch of different features in the settings section. The invidious links option parses the downloaded github page. Can be updated by just replaceing the html file with the redownloaded invidious html page. Can change a lot of the settings in the config files. Some ideas for the future 1)might at m3u 2)maybe nlp for categories 3) maybe feedreading stuff. Try not to go to overboard though.

-------------------------------------------
Hidden bookmarks
-------------------------------------------
There is a password protected Bookmarks section which can only be accessed by typing @secret or @hidden into the main form. To add new pages to this section, you would type something like https://www.google.com@secret or https://www.google.com@hidden  . To just view the section you would only type @secret or @hidden into the main form. You are offered the option to change the passphrase. After it has been changed, hidden bookmarks can be added with password https://www.google.com . It's just your created password followed by a space and then the url you are adding. To access the hidden bookmarks with the new password, you just type in the password. You don't need the @ symbol if you created a password. You can now move bookmarks from the main section to the password section by editing the bookmark and adding you password before it. It will move it between the two sections. in case you accidentally added something you wanted in the password section to the main page. It sorts nsfw into the password protected section based off a file put together by nofap lol. You can change the default behavior by modifying that file.

1)To import your bookmarks, go to firefox>bookmarks>manage bookmarks>import and backup>click on backup

2)then open that in the applications file picker.

3)It will probably take a second. That's the application trying to pull out images and sorting out NSFW content.

If you don't provide information about a website, it will try and scrape it. Kinda doubt there would be enough requests to cause any problems.

If you try and import your bookmarks a second time, it will only add the new bookmarks. So you can update it by importing your firefox bookmarks multiple times. 

-------------------------------------------
Downloads
-------------------------------------------
*The windows application needs to be repackaged with latest updates

windows 
download link= https://icedrive.net/s/g62kVCYYfghSCZbu2fB53tfY7h7A

linux 
download link= https://icedrive.net/s/AVQGQy1D9k5R3vyiuY4kiftkRRB3

The android application is hosted on github.
----------------------------------------
I quit working on the android application a while back. Got tired of repackaging it over and over again on a bunch of systems. You can probably still run what i had at the time. If you are curious about pythonforandroid, shows that it can be ported to android. 




