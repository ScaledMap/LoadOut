

![Alt text](https://github.com/ScaledMap/LoadOut/blob/main/Screenshot%20from%202022-05-16%2010-06-16.png?raw=true "Main bookmarks page for the application")

Still a work in progress. 

This application gets updated somewhat frequently  with small updates. To keep your database without having to redo everything, just redownload the application and overwrite the bookmarks.sqlite file with the old bookmarks.sqlite file. Can also move your notes over by overwriting the notes folder.

-------
Loadout
-------

LoadOut is a Bookmark manager I've been working on to help manage and organize my bookmarks. It's a Pywebview application built on flask. You can run it as a server or as a webview. It allows you to import your bookmarks from firefox and create categories to interact with those bookmarks. It would also probably be useful for situations where you want to avoid messing with the keyboard. There was a time where i was using opera because speeddial was useful. I'd kind of like it to be a more flexible alternative to something like pocket or speedial. It should work with most browsers. There is also the added benefit of not having to make an account. If you decide to set it up as a server, it's a cool way to get all your web data on all of your devices.

Categorized and organized bookmarks in any browser, as a server, or as an application

![Alt text](https://github.com/ScaledMap/LoadOut/blob/main/server%20or%20webview.png?raw=true, "The add bookmarks page. It will pull out urls from your clipboard if that setting is turned on and you can update it by just reimporting your bookmarks.")

create a category, choose a background icon and pick a color

![Alt text](https://github.com/ScaledMap/LoadOut/blob/main/categories.png?raw=true "create, add icons, color coordinate and edit categories")

-------------------------------------------
Downloads
-------------------------------------------



   
windows 
*The windows application needs to be repackaged. it's way, way behind the linux builds
download link= https://icedrive.net/s/g62kVCYYfghSCZbu2fB53tfY7h7A


linux 
*mainly tested on debian systems. Working on testing it on manjaro.
download link= https://icedrive.net/s/fAwV3u6f3aDfT3v71Rtt4uW15iSG


raspberry pi
download link = https://icedrive.net/s/Nz4gvN36kNuYkDTY2XuX3PBAfRTy


--------------
Installation
--------------
You don't have to install anything. Just download and unzip the provided folder. The executable should be at the bottom of that folder. You are looking for loadout.exe or just loadout. 

--------------
Utility
-------------
My advice would be to run the application as a server. You can set it up to run the server at startup or you can change the icon. The application will open the default browser when you click the executable if it's set to run as a server. there is also a new tab extension available for firefox. Can have newtabs default to a specific port.

One benefit of this application is that it will work with most browsers. Some of the more privacy focused browsers don't do cookies by default. This would be really useful with something like librewolf.

If you decide to run the application as a server, Pywebview doesn't default to persistent cookies. History won't show up when you open links in the webview. The application will save bookmarks created while using the webview's browser to a seperate category called webview. if you are into stumbleupon(guess its "cloudhiker now... lol lost the domain"), the webview is an option for keeping your bookmarks seperate.
Running the program as a server makes it easy to keep the same set up on all of your devices/browsers.

I use this application on a daily basis. Some of the categories I've come up with are:

backing tracks, guitar practice, guitar tabs(if you don't know what tabs are, they are a form of music notation for guitar) literature, weird, Random videos, javascript, learn programming(could fork this into python learning tools, python info, other programming languages), exercise, art, iptv, streaming, pick up later(where I left off in a show or video), gaming, argg 

---------------------------------


-------
features
-------
In adition to the stuff already mentioned


1) You can import your bookmarks into the application from firefox. 

2) The program will automatically sort out any images, youtube videos or youtube channels. If you don't currently have any youtube channels, videos or images, this gives you an easy way of saving and organizing those items.

3) You can update the application by importing your bookmarks multiple times. Since the program wont let you upload the same bookmarks multiple times, you can update the application by just reimporting your bookmarks.

4) You can choose the default page for the application. If there are some links you use more than others, you can set it so that category shows up when the program launches.  

5) The youtube channels section lists all your saved youtube channels or bookmarked channels. A button in that section will pull out a list of random videos. lol sometimes you just want something playing. also a good way to keep track of stuff if you are a "privacy guy". I'd usually prefer to not have accounts.

6) There is a really basic download option for videos in the youtube videos section. 

7) There is a note taking app. Each category has it's own note taking app. To get to the app click on the yellow button on the bookmarks page and then click notes. You can also obfuscate the text. Only one option is currently available though.

8) convert youtube links and reddit links into invidious and libreddit links. It will pull up one of the instances at random. Makes it easy to not have to think about going to those privacy alternatives. 

9) If you add a youtube video to the application, the application will recognize that it's a youtube video and a playlist option with show up in that category. When you click on the playlist button, the application will automatically start playing all the videos in that category as a playlist. Really barebones option for music playlists or anything else you would need a playlist for. 

10) You can shorten urls and save the shortened links. 


Might be better to just look at the settings page below.

![Alt text](https://github.com/ScaledMap/LoadOut/blob/main/settings.png?raw=true "list of application settings")

As of now,these are the customization options currently available in the program.

![Alt text](https://github.com/ScaledMap/LoadOut/blob/main/customization_settings.png?raw=true "customizing the application")


basic usage:
----------------

Images

to add images open image in new tab, open image link, open image, etc. You want the link that has the image type in it. png, gif, svg, etc. its usually better to pull images out of websites directly. googles images, and bing images, etc. are a work in progress. 

Should support any filetype listed on firefox's documentation.

Youtube

looks for youtube.com/watch or youtube.com/embed to filter iframes and construct playlists out of categories

youtube channels

It will filter out /channel/, /c/ and /user/ urls into the channels category. 

type @secret or @hidden in the main +website form to open the protected bookmarks
@secret or @hidden == default passwords

so yeah... Kind of gives your bookmarks more utility. 
![Alt text](https://github.com/ScaledMap/LoadOut/blob/main/Videos.png?raw=true, "download, play, embed and link to videos")


-------------------------------------------
Hidden bookmarks
-------------------------------------------
There is a password protected Bookmarks section which can only be accessed by typing @secret or @hidden into the main form(the one with the https:// placeholder). To add new pages to this section, you would type something like https://www.google.com@secret or https://www.google.com@hidden To just view the section, you would only type @secret or @hidden into the main form. You are also offered the option to change the passphrase after you log in. After it has been changed, hidden bookmarks can be added with   password https://www.google.com  . It's just your created password followed by a space and then the url you are adding. To access the hidden bookmarks with the user created password, you just type the password into the main form. You don't need the @ symbol if you created a password. You can also move bookmarks from the main section to the password section by editing the bookmark and adding you password before the url in the url field. Just like you would add a new url to the password protected section.

When you import your bookmarks, it will sort out any nsfw content. it sorts out nsfw content into the password protected section based off a file put together by nofap lol. You can change the default behavior by modifying that file. Search engines aren't filtered out by default and imgur is at the moment. You can modify the file to change what sites are filtered.

![Alt text](https://github.com/ScaledMap/LoadOut/blob/main/protected-bmark.png?raw=true, "Hidden bookmarks and images")

--------------------
importing your bookmarks
--------------------

1)To import your bookmarks, go to the firefox settings button>bookmarks>manage bookmarks>import and backup>click on backup

2)then open that json file in the application's file picker found under the settings link.

3)It will probably take a second. That's the application trying to pull out images and sorting out NSFW content.

If you don't provide information about a website, it will try and scrape the website. Kinda doubt there would be enough requests to cause any problems. Think it's only 1 request per bookmark. If it doesn't find anything, you can change anything you want later. 

If you try and import your bookmarks a second time, it will only add your newly added bookmarks. You can update the application by importing your firefox bookmarks multiple times. 


The android application is hosted on github.
----------------------------------------
I quit working on the android application a while back. Got tired of repackaging it over and over again on a bunch of systems. You can probably still run what i had at the time. If you are curious about pythonforandroid, shows that it can be ported to android. I was a little further along then what is shown there. Also shows why it's taken a while to get an application running. Was going to be a password manager. I was packaging it on linux, windows, android, as a server and a webview. The application behaves differently between running as webview and a server.

Part of this was me playing around with pywebview. The application uses both the flask pywebview api and the pywebview javascript api. Figured mine as well try out the non flask option. Android was kind of an afterthought.

Todo list
----------------------------------------------
fix redirects for libreddit, add an export bookmarks button. Add filters for search engine proxies. Clean up the readme. Might start with rss reader that just works for reddit links. Mess with the channels section or the download option

![Alt text](https://github.com/ScaledMap/LoadOut/blob/main/Screenshot%20from%202022-05-16%2009-45-06.png?raw=true, "cardview page for jumping around quickly and accessing your notes")


most recent updates
-------------------

Fixed a lot of bugs and been messing with it on arch

Converting to libreddit is working a lot better. There was also an issue accessing it from the cardview. I got playlists working on custom categories that are set as the index(homepage). I added an html color picker into the application. Kept the link to w3. The settings will update automatically now. Don't have to reload the application. Notes are working. Bunch of small updates. 

pyperclip wasn't working for a second. It isn't working on the pi and the exception wasn't working on linux for some reason. Fixed that. Might try and leave up more than one version at a time in the future

Also, restore to default settings isn't working atm. I'm kind of okay with that. Removing the database file will force the application to restore the original default values from a long time back "bookmarks.sqlite". I'd kind of prefer to redo that button anyway. I know what broke it. Just the redirects. It didn't work properly on windows the way it was set up. Wasn't a great solution in general.

updated the normal linux build. I'm going to do another build for the pi before i upload that. There is a bug that is pretty annoying in the last build. There has been a warning going off saying set track_modifcations in config. Finally got tired of that and it seems like it made things run a lot faster.

Also, I added hidden categories. <password> <url> <category>

The category has to be 1 word atm. Will probably set it up to take quotes later. The form in the password section takes 2 arguments now. <url> <category> Obviously you leave out the <>. just space seperated arguments. You can filter out nsfw bookmarks completly now when importing from firefox. Sure nofap would be happier about that lol. Did use their giant, giant list. To tell it to throw out nsfw bookmarks, you need to go to the password protected bookmarks and edit the settings in there. It defaults to how it had been running. It also wont let you reimport the same hidden bookmarks more than once now. Just fixed a lot of little things. Seperated notes into a seperate folder. Might do that with the config files as well. The hidden bookmarks aren't super flushed out. Can only add to those categories by retyping the category name more than once. Will make editing the hidden bookmarks an option when I get a chance. I will also add them to the other dropdown.

I was able to get the webview working. There are a few issues with running the application as a webview. Will kind of pick at fixing the bugs. Figured I'd remove the part about qtwebengine at least since I did get it kind of working. Pyperclip doesn't work. Also the descriptions aren't showing up.

Mainly updated this because I wanted to remove stuff about qtwebengine. At the time, I had run into an article online saying qtwebengine wouldn't work on the pi. It might be causing the bug with the descriptions, but things will work for the most part. Anyway, I will upload the updated pi build build in a few days. 

hostname -I to pull up the ipaddress in bash

The server should definetly work on all your devices now. I might add an option where you can choose to have the server just run in your browser vs allowing other devices to connect.



