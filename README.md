# LoadOut
LoadOut is an application I've been working on to help manage and organize my bookmarks. It's a Pywebview application built on flask. You can run it as a server or as a webview.  It allows you to import your bookmarks from firefox and create categories to interact with those bookmarks. It would also probably be useful for situations where you want to avoid messing with the keyboard. I had a setup at one point where i was using opera because speeddial was useful when I was hooked up to the TV. It meant I didn't need to use the keyboard as much. This is, and has, been useful in a similar usecase. I've found that LoadOut has the most utility when run as server and set as your homepage. If you just wan't to use the webview though, there are some perks with that as well. The webview runs on chromium and doesn'[t remember cookies. Don't thank me, thank the pywebview guy lol. 

There are a lot of things I could probably do with this application in the future. hope I continue to work on it. More customization would be nice. More default filters. I was thinking about trying to add rss. A rss server sounds pretty cool. 


downloads are available as onefile or a download where the ini files are visible.
------------------------------------

windows 
download link= https://icedrive.net/s/g62kVCYYfghSCZbu2fB53tfY7h7A

linux 
download link= https://icedrive.net/s/g4SD5G5TuyyvkB36X9jGiYug68g2

The android application is hosted on github.
----------------------------------------
I quit working on it a ways into the project. Got tired of repackaging it over and over again on a bunch of systems. The core application works on android. I may go back and try and get everything working on android. The android application lets you keep track of your bookmarks, but it can't import them from firefox. It's been kind of useful but it's nothing amazing.


----------------------------------------
about
-----------

There is a password protected Bookmarks section which can only be accessed by typing @secret or @hidden into the main form. To add new pages to this section, you would type something like https://www.google.com@secret or https://www.google.com@hidden  . To just view the section you would only type @secret or @hidden into the main form. You are offered the option to change the passphrase. After it has been changed, hidden bookmarks can be added with password https://www.google.com . It's just your created password followed by a space and then the url you want to add. To access the hidden bookmarks with the new password, you just type in the password. You don't need the @ symbol if you created a password. I planned on adding a password manager. I will probably try to add a bunch of stuff. At the very least, I  at least have it to a point where everything seemsto function as intended. Wanted to at least have something I could upload. 

Couldnt be easier to use

Just unzip the files and click on the executable. It should be the last file in the folder if it's sorted alphabetically. There's probably more security with the onefile packages. It's nice to be able to mess with the ini files though. If it's not working, we could try using the one the runs with the terminal.

1)To import your bookmarks, go to firefox>bookmarks>manage bookmarks>import and backup>click on backup
2)then open that in the applications file picker.
3)It will probably take a second. I haven't built a loading secreen : \ just give it a sec. It's trying to pullout the favicons and everything. It should also sort out nsfw content if it finds it.

If you don't provide information about5 a website, it will try and scrape it. Kinda doubt there would be enough requests to cause in problems.

If you try and import your bookmarks a second time, it will only add the new bookmarks. So you can update it by importing your firefox bookmarks if you wanted to. Yeah. cool stuff. lol also going to work on the add icon sections.

