# LoadOut


LoadOut is a Bookmark manager I've been working on to help manage and organize my bookmarks. It's a Pywebview application built on flask. You can run it as a server or as a webview.  It allows you to import your bookmarks from firefox and create categories to interact with those bookmarks. It would also probably be useful for situations where you want to avoid messing with the keyboard. There was a time where i was using opera because speeddial was useful. I'd kind of like it to be a more flexible alternative to something like pocket or speedial. Still kind of a work in progress. I'll probably upload the python script in a bit and a list of packages(requirments.txt) if the exe is too much. Kind of just pick at it when i get bored. Add stuff I think is cool. It could use some optimization. Runs well enough though. My advice would be to run it as a server. You can set it up to boot at startup and set it as the load in page(like how pocket would usually load in). An alternative idea would be to change the icon and run it as a server. When it's set as a server, it will open the default browser when u click on the icon.In the photos section, the desktop is cinnamon. Figure people might wonder about that. 

There are a lot of things I could probably do with this application in the future. More customization would be nice. More default filters. I was thinking about trying to add rss.

----------------------------------------
about and updates
-----------------------------------------
The linux application has been updated. The windows application is way behind the linux build at the moment

edit may 14:Fixed a bug with the filepicker. Added A bigscreen mode that kind of looks like speeddial. It isn't set as the default loadin because it looks a little wonky if there arent many bookmarks in a category. Added the foundation for a feedreading webapp. refractored the application a bit. Going to rearange the database around images and rss. 

edit may 13:Added a default background image. edit:made background image fixed. You can switch it back to colors as the default backtround in the customize.ini file. Set the [background-image][image]= None. Without quotes. You can also change the background image this way. It will add whatver path you write in. Fixed a bug where order wasn't working when loaded from the cardview. Added a notetaking webapp to the project. YOu can create notes based on category in the cardview section(might add an option for basic encryption/obfiscation for notes). The application ill open reddit links with a random libreddit instance now(still need to clean that code up a bit. Ideally everything could be tweaked from the files). It's the same button as "convert youtube to invidious" Will probably add settings for this and the background image. You can also add bookmarks to the application from the webview now. importing bookmarks is still probably the best option though. 

features/updated

atomatically sorts out images. Added navigation options if you want to open up a url inside a webview. Sorts out youtube channels by default. You can see the most recent videos on bookmarked youtube channels. Added an option to open youtube links in a random invidious instance. Added a search bar to search through all your bookmarks/search bar for icons. There is a cardview section which is an alternative to using the dropdown. You can choose what bookmarks open when the application is loaded. You can choose what page is loaded in general. Most of the features are in the settings section. If it looks really plane, there is a change i accidentally packaged it with all the settings disabled or something. The invidious links option parses the invidious instance list. You can be update it by just replaceing the html file with the redownloaded invidious instance list https://redirect.invidious.io/. Save page and overwrite. For example I think the kevinrocks instance is dead. Can change a lot of the settings in the config files. 




todo
----------------------
Some ideas for the future
1)might add m3u support
2)maybe nlp for categories 3) 
3)feedreading stuff.


Try not to go to overboard though.
really need to get things together with version control. I didn't really originally plan on it being as comprehensive as it currently is. Think running it as a server is what makes it a pretty great idea for an application.

-------------------------------------------
Hidden bookmarks
-------------------------------------------
There is a password protected Bookmarks section which can only be accessed by typing @secret or @hidden into the main form(the one with the https:// placeholder). To add new pages to this section, you would type something like https://www.google.com@secret or https://www.google.com@hidden  . To just view the section, you would only type @secret or @hidden into the main form. You are also offered the option to change the passphrase. After it has been changed, hidden bookmarks can be added with   password https://www.google.com  . It's just your created password followed by a space and then the url you are adding. To access the hidden bookmarks with the new password, you just type in the password. You don't need the @ symbol if you created a password. You can now move bookmarks from the main section to the password section by editing the bookmark and adding you password before it. Just like you would add a new url to the password section. edit the url value and then password https://www.digg.com . lol something like that. It will move it between the two sections. Just in case you accidentally added something you wanted in the password section to the main page. It sorts out nsfw content into the password protected section based off a file put together by nofap lol. You can change the default behavior by modifying that file. Search engines are filtered out by default and imgur is at the moment. Can just open the file an delete that url to change it. 

1)To import your bookmarks, go to firefo settings buttonx>bookmarks>manage bookmarks>import and backup>click on backup

2)then open that json file in the applications file picker.

3)It will probably take a second. That's the application trying to pull out images and sorting out NSFW content.

If you don't provide information about a website, it will try and scrape it. Kinda doubt there would be enough requests to cause any problems(if you are worried about the servers, chill out man... It's like... 1 request per bookmark. )

If you try and import your bookmarks a second time, it will only add the new bookmarks. You can update it by importing your firefox bookmarks multiple times. 

-------------------------------------------
Downloads
-------------------------------------------
*The windows application needs to be repackaged with latest updates

windows 
download link= https://icedrive.net/s/g62kVCYYfghSCZbu2fB53tfY7h7A

linux 
download link= https://icedrive.net/s/3vVj8Zh5v3Zjb1x2ZWiB5FD2yu1w


The android application is hosted on github.
----------------------------------------
I quit working on the android application a while back. Got tired of repackaging it over and over again on a bunch of systems. You can probably still run what i had at the time. If you are curious about pythonforandroid, shows that it can be ported to android. I was a little further along then what is shown there. Also shows why it's taken a while to get an application running. Was going to be a password manager. Just changed a lot.

Todo list
----------------------------------------------

improve how it scrapes libreddit, fix up "speeddial" page behaves properly without a bunch of bookmarks, continue working on feedreader, think if i decide to add m3u support it'd probably be through vlc, WORK UP THE NERVE TO PUBLISH THE APPLICATION, clean up the positioning on a few of the pages, look into messing with selenium(would maan the application would break without updates), add the libreddit instance setting as its own button, add filepicker or at least form to update the background image(instead of the customize.ini file), look into porting the application to mobile(probably with an api and kivy)




