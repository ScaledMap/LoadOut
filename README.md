# LoadOut
LoadOut is an application I've been working on to help manage and organize my bookmarks. It's a Pywebview application built on flask. You can run it as a server or as a webview.  It allows you to import your bookmarks from firefox and create categories to interact with those bookmarks. It would also probably be useful for situations where you want to avoid messing with the keyboard. I had a setup at one point where i was using opera because speeddial was useful when I was hooked up to the TV. This has been useful in similar usecases.

There are a lot of things I could probably do with this application in the future. hope I continue to work on it. More customization would be nice. More default filters. I was thinking about trying to add rss. An rss server sounds pretty cool.


downloads are available as onefile or a download where the ini files are visible.
------------------------------------


--------------------
*maybe hold off on using the onefile version of the application. It can't read from the config file. If I try to reupload the onefile version, I think I will probably have to move those settings into a database or something(not building it on windows). Also, seems like the application can have some trouble opening a browser window to localhost on startup. Might have to type it in. Setting it as the home page is a cool way to do it anyway. Problems don't exist on linux.
*I guess Icedrive zipped the folders again after I had already zipped them. So for the windows application, i think you have to unzip them and unzip them.
-----------------------

windows 
download link= https://icedrive.net/s/g62kVCYYfghSCZbu2fB53tfY7h7A
linux 
download link= https://icedrive.net/s/g4SD5G5TuyyvkB36X9jGiYug68g2

The android application is hosted on github.
----------------------------------------
I quit working on it a ways into the project. Got tired of repackaging it over and over again on a bunch of systems. 


----------------------------------------
about
-----------

There is a password protected Bookmarks section which can only be accessed by typing @secret or @hidden into the main form. To add new pages to this section, you would type something like https://www.google.com@secret or https://www.google.com@hidden  . To just view the section you would only type @secret or @hidden into the main form. You are offered the option to change the passphrase. After it has been changed, hidden bookmarks can be added with password https://www.google.com . It's just your created password followed by a space and then the url you want to add. To access the hidden bookmarks with the new password, you just type in the password. You don't need the @ symbol if you created a password. I planned on adding a password manager. I will probably try to add a bunch of stuff. At the very least, I at least have it to a point where everything seemsto function as intended. Wanted to at least have something I could upload. 

Couldnt be easier to use


Just unzip the files and click on the executable. It should be the last file in the folder if it's sorted alphabetically(loadouts.exe). There's probably more security with the onefile packages. It's nice to be able to mess with the ini files though(forgetting what port you are running it on and stuff). If it's not working, we could try use the ones that run in the terminal.

1)To import your bookmarks, go to firefox>bookmarks>manage bookmarks>import and backup>click on backup
2)then open that in the applications file picker.
3)It will probably take a second. I haven't built a loading secreen :\ just give it a sec. It's trying to pull out the favicons and everything. It should also sort out nsfw content if it finds any. It does that based off the domain. Search engines arn't sorted out.

If you don't provide information about5 a website, it will try and scrape it. Kinda doubt there would be enough requests to cause any problems.

If you try and import your bookmarks a second time, it will only add the new bookmarks. So you can update it by importing your firefox bookmarks multiple times. 

-----------------------------------------
Even if you don't really feel the application would be all that useful. The default bookmarks i have set up are kind of great. Stumbleupon(god i used to love that), literally like every guitar scale ever, python tutorials. Keeping track of my backing tracks is nice too.
