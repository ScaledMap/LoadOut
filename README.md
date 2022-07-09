
most recent updates
-------------------

The server should definetly work on all your devices now. I might add an option where you can choose to have the server just run in your browser vs allowing other devices to connect.

Updated the raspberry pi build. It should be at the same place in development as the normal linux build. I'm in the unusual situation where my main computer is hardwired and doesn't have a wireless card. I was able to run the application as a server while messing with it on the pi. So at this point at least, pretty confident that the server will run on all your other devices. It really was pretty cool having all my webstuff right there on all the devices at my dads house. I'm pretty psyched about working on this project after getting the raspberry pi server going. It was cool being able  to pull up my music playlists on all the devices in the house. Cool seeing it on mobile. After messing with the networking side of things, I think I will probably try and add some kind of loose account settings eventually. I guess you could just run the application on two different ports? ¯\_(ツ)_/¯. I'll test how that works.

Unfortunitely, I don't think getting the webview to work is an option on the raspberry pi. The raspberry pi doesnt support QtWebEngine. You can get pywebview to work with QtWebKit, but pyinstaller doesn't like using QtWebKit. It has depreciated it. Maybe an option would be to use an older version of pyinstaller. I'm probably not going to make that a huge priority though.  Gtk might also be an option. I also had to use some depreciated libraries to get that to work. It can run as a webview on the raspberry pi if I don't package it. Kinda makes more since as a server on the pi anyway though. So yeah. Not at the top of my to do list.

Also, raspbian unfortunitely won't work either. I built the raspberry pi build on raspberry pi os. I could try doing a build for raspbian i guess. Maybe if i get bored.

![Alt text](https://github.com/ScaledMap/LoadOut/blob/main/Screenshot%20from%202022-05-16%2010-06-16.png?raw=true "create, add icons, color coordinate and edit categories")

-------
Loadout
-------

LoadOut is a Bookmark manager I've been working on to help manage and organize my bookmarks. It's a Pywebview application built on flask. You can run it as a server or as a webview.  It allows you to import your bookmarks from firefox and create categories to interact with those bookmarks. It would also probably be useful for situations where you want to avoid messing with the keyboard. There was a time where i was using opera because speeddial was useful. I'd kind of like it to be a more flexible alternative to something like pocket or speedial. It should work with most browsers. If you decide to set it up as a server, it's a cool way to get all your web data on all of your devices. I'm kind of working on this project because 1) I wanted something like this 2) I kind of just like computer programming. 

Categorized and organized bookmarks in any browser, as a server or as an application

![Alt text](https://github.com/ScaledMap/LoadOut/blob/main/server%20or%20webview.png?raw=true, "Main bookmarks page for the application")

create categorize, choose background icon and color

![Alt text](https://github.com/ScaledMap/LoadOut/blob/main/categories.png?raw=true "create, add icons, color coordinate and edit categories")?raw=true "create, add icons, color coordinate and edit categories")



--------------
Utility
-------------
My advice would be to run it as a server. You can set loadout to boot at startup and make it your homepage.  Another option would be to change the icon(so it looks like firefox or whatever your default browser is) and run it as a server. it will try and open your default browser when you click on the exe.

You could also use this with librewolf or an alternative browser. Some of the more privacy focused browsers don't do cookies by default. This would be really useful with something like librewolf.

You could also use the webview as a browser. Kind of a limiting experience but you could try it. Pywebview doesn't default to persistent cookies. History won't show up when you open links in the webview. Stumbleupon(guess its "cloudhiker now... lol lost the domain") works well in the webview. You can add bookmarks through the webview like you normally would in the browser. Works well if you want to keep stumbleupon stuff seperate from normal bookmarks.

-------
features
-------
In adition to the stuff already mentioned. You can import your bookmarks into the application from firefox. The program will automatically sort out any images, youtube videos or youtube channels. You can update the application by reimporting your bookmarks into the application. The program won't let you add the same bookmarks so you can keep things updated by reimporting your bookmarks multiple times or from all your browsers. If you don't currently have any youtube channels, youtube videos or images in your bookmarks, going forward you will have an easy way of saving and organizing all those items. The youtube channels section will list all youtube channels you had in your bookmarks. When you click on the videos button in that tab, the program will load some of that videos from that creator. Good way to keep track of stuff if you are a "privacy guy". I'd usually prefer to not have accounts. This would also save your stuff so it could potentially be accessed anywhere on the network. The youtube videos option will import yout youtube videos. There is a really basic download option for the videos in the youtube videos section. The application also has an option in the settings to convert youtube links and reddit links into invidious and libreddit links. Makes it easy to not have to think about going to those privacy alternatives. Might look into adding more of these redirects as settings. If you add a youtube video to the application, the application will recognize that it's a youtube video and a playlist option with show up in that category. When you click on the playlist button, the application will automatically start playing all the videos in that category. Really barebones option for music playlists. You can use this for anything you would need a playlist for. You can also shorten urls and save the shortened links. 

Might be better to just look at the settings page below. You can also shorten urls and save the shortened links.

![Alt text](https://github.com/ScaledMap/LoadOut/blob/main/settings.png?raw=true "list of application settings")

These are the customization options currently in the program

![Alt text](https://github.com/ScaledMap/LoadOut/blob/main/customization_settings.png?raw=true "customizing the application")



-------------------------------------------
Downloads
-------------------------------------------
*The windows application needs to be repackaged with latest updates

*only the server is working on the pi. I'm having trouble with the webview. I've had issues with python packages on raspberry pi in the past. Might just modify it so the server is the only option.

windows 
download link= https://icedrive.net/s/g62kVCYYfghSCZbu2fB53tfY7h7A

linux 
download link= https://icedrive.net/s/XT5R8G3BxTZBT2vQZYxZC1tPykQf

raspberry pi/ARM 32
download link = https://icedrive.net/s/Nz4gvN36kNuYkDTY2XuX3PBAfRTy




basic usage:
----------------
I usually do pretty much everything on the web at point. This type if thing works great for how i use computers

you can add anything you want but these urls will be sorted into the appropriate categories by default.



Images


to add images open image in new tab/open image link/. its usually better to pull images out of websites directly. googles images, and bing images, etc. are a work in progress. 

Should support any filetype listed on firefox's documentation.



Youtube

looks for youtube.com/watch or youtube.com/embed to filter iframes and construct playlists out of categories



youtube channels

It will filter out /channel/, /c/, /user/ urls into the channels category. From the category you can pull out random vidoes from the channel. Some people are never going to be ok with making accounts. least you can save the channels somewhere.



type @secret or @hidden in the main +website form to open the protected bookmarks
@secret or @hidden == default passwords


so yeah... Kind of gives your bookmarks more utility. 


-------------------------------------------
Hidden bookmarks
-------------------------------------------
There is a password protected Bookmarks section which can only be accessed by typing @secret or @hidden into the main form(the one with the https:// placeholder). To add new pages to this section, you would type something like https://www.google.com@secret or https://www.google.com@hidden . To just view the section, you would only type @secret or @hidden into the main form. You are also offered the option to change the passphrase. After it has been changed, hidden bookmarks can be added with   password https://www.google.com  . It's just your created password followed by a space and then the url you are adding. To access the hidden bookmarks with the new, user created password, you just type the password into the main form. You don't need the @ symbol if you created a password. You can also move bookmarks from the main section to the password section by editing the bookmark and adding you password before the url in the url field. Just like you would add a new url to the password protected section. I

It sorts out nsfw content into the password protected section based off a file put together by nofap lol. You can change the default behavior by modifying that file. Search engines aren't filtered out by default and imgur is at the moment. You can modify the file to change what sites are filtered.

1)To import your bookmarks, go to the firefox settings button>bookmarks>manage bookmarks>import and backup>click on backup

2)then open that json file in the application's file picker found under the settings link.

3)It will probably take a second. That's the application trying to pull out images and sorting out NSFW content.

If you don't provide information about a website, it will try and scrape the website. Kinda doubt there would be enough requests to cause any problems. Think it's only 1 request per bookmark.

If you try and import your bookmarks a second time, it will only add your newly added bookmarks. You can update the application by importing your firefox bookmarks multiple times. 


The android application is hosted on github.
----------------------------------------
I quit working on the android application a while back. Got tired of repackaging it over and over again on a bunch of systems. You can probably still run what i had at the time. If you are curious about pythonforandroid, shows that it can be ported to android. I was a little further along then what is shown there. Also shows why it's taken a while to get an application running. Was going to be a password manager. I was packaging it on linux, windows, android, as a server and a webview. The application behaves differently between running as webview and a server.

Part of this was me playing around with pywebview. The application uses both the flask pywebview api and the pywebview javascript api. Figured mine as well try out the non flask option. Android was kind of an afterthought.

Todo list
----------------------------------------------
fix redirects for libreddit, add an export bookmarks button. Add filters for search engine proxies. Clean up the readme. Might start with rss reader that just works for reddit links. Mess with the channels section or the download option

![Alt text](https://github.com/ScaledMap/LoadOut/blob/main/Screenshot%20from%202022-05-16%2009-45-06.png?raw=true)
