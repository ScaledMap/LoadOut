# LoadOut
LoadOut is an Bookmark manager I've been working on to help manage and organize my bookmarks. It's a Pywebview application built on flask. You can run it as a server or as a webview.  It allows you to import your bookmarks from firefox and create categories to interact with those bookmarks. It would also probably be useful for situations where you want to avoid messing with the keyboard. I had a setup at one point where i was using opera because speeddial was useful when I was hooked up to the TV. This has been useful in similar usecases.

There are a lot of things I could probably do with this application in the future. hope I continue to work on it. More customization would be nice. More default filters. I was thinking about trying to add rss. An rss server sounds pretty cool.


downloads are available as onefile or a download where the ini files are visible.
------------------------------------
The linux application has been updated. Added a few settings. atomatically sorts out images. Some navigation options if you want to open up a url inside the webview. Sorts out youtube channels by default. Can see the most recent videos on the channels. ONly the linux non one file version is currently updated.


*maybe hold off on using the onefile version of the application. It can't read from the config file.
*I guess Icedrive zipped the folders again after I had already zipped them. So for the windows application, i think you have to unzip them and unzip them again.


windows 
download link= https://icedrive.net/s/g62kVCYYfghSCZbu2fB53tfY7h7A

linux 
download link= https://icedrive.net/s/g4SD5G5TuyyvkB36X9jGiYug68g2

The android application is hosted on github.
----------------------------------------
I quit working on the android application a while back. Got tired of repackaging it over and over again on a bunch of systems. 


----------------------------------------
about
-----------

There is a password protected Bookmarks section which can only be accessed by typing @secret or @hidden into the main form. To add new pages to this section, you would type something like https://www.google.com@secret or https://www.google.com@hidden  . To just view the section you would only type @secret or @hidden into the main form. You are offered the option to change the passphrase. After it has been changed, hidden bookmarks can be added with password https://www.google.com . It's just your created password followed by a space and then the url you want to add. To access the hidden bookmarks with the new password, you just type in the password. You don't need the @ symbol if you created a password. I planned on adding a password manager. I will probably try to add a bunch of stuff. I Wanted to at least have something I could upload. 

1)To import your bookmarks, go to firefox>bookmarks>manage bookmarks>import and backup>click on backup
2)then open that in the applications file picker.
3)It will probably take a second. I haven't built a loading secreen :\ just give it a sec. It's trying to pull out the favicons and everything. It should also sort out nsfw content if it finds any. It does that based off the domain. Search engines arn't sorted out.

If you don't provide information about a website, it will try and scrape it. Kinda doubt there would be enough requests to cause any problems.

If you try and import your bookmarks a second time, it will only add the new bookmarks. So you can update it by importing your firefox bookmarks multiple times. 

