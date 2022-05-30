Hosting the file on icedrive until i publish it

basic usage:
----------------
open image in new tab/open image link .jpeg/.gif, etc = images(can work with some proxies)
youtube.com/watch/ = to create playlists and filter iframes
/channel/ = to pull out the bookmarked channel

it can pull these out of your bookmarks or you can just add them directly to the application
@secret/@hidden = default password

you can add anything you want but those urls will be sorted into the appropriate categories by default. so yeah... Kind of gives your bookmarks more utility. 

Title
-------
Loadout
-------

LoadOut is a Bookmark manager I've been working on to help manage and organize my bookmarks. It's a Pywebview application built on flask. You can run it as a server or as a webview.  It allows you to import your bookmarks from firefox and create categories to interact with those bookmarks. It would also probably be useful for situations where you want to avoid messing with the keyboard. There was a time where i was using opera because speeddial was useful. I'd kind of like it to be a more flexible alternative to something like pocket or speedial. My advice would be to run it as a server. You can set loadout to boot at startup and make it your homepage.  Another option would be to change the icon(so it looks like firefox) and run it as a server. it will try and open your default browser when you click on the exe if its set to run as a server.

You could also use this with librewolf or an alternative browser. Some of the more privacy focused browsers don't do cookies by default. Bookmarks would be useful in that case.

You could also use the webview as a browser. Kind of a limited experience but you could try it.

----------------------------------------
 updates
-----------------------------------------
The linux application has been updated. The windows application is way behind the linux build at the moment

edit may 30: the music category now has an option to open your youtube links in that category in a playlist. Kind of a clever solution to putting together a simple way to play music. Way easier than selenium or using the api. Cleaned up the images section. can edit and remove images from the images section. Cleaned up a bunch of bugs. Images only show up if they are added to the photos category at the moment. That isn't the ideal behavior I just need to think about how i handle that for a bit. Also added basic obfiscation to the notes webapp. You can convert the notes back and forth between plain text and the encoding. probably add more encodings later.

edit may 16: changed the background for the categoriess section. It can be adjusted in the customize.ini file. Design feels 100 percent better now. I have a ton of bookmarks so sometimes bugs slip through when i test it without my bookmarks in the database.

edit may 14:Fixed a bug with the filepicker. Added A bigscreen mode that kind of looks like speeddial. It isn't set as the default loadin because it looks a little wonky if there arent many bookmarks in a category. Added the foundation for a feedreading webapp. refractored the application a bit. Going to rearange the database around images and rss. 

edit may 13:Added a default background image. edit:made background image fixed. You can switch it back to colors as the default backtround in the customize.ini file. Set the [background-image][image]= None. Without quotes. You can also set the bookmarks background image this way. It will add whatver path you write in the .ini file. Fixed a bug where order wasn't working when loaded from the cardview. Added a notetaking webapp to the project. YOu can create notes based on category. This is in the cardview section(might add an option for basic encryption/obfiscation for notes). The application will open reddit links with a random libreddit instance now(still need to clean that code up a bit. Ideally everything could be tweaked from the files). It's the same button as "convert youtube to invidious". You can add bookmarks to the application from the webview now. importing bookmarks from firefox is still probably the best option though. 


-------
features/
-------
atomatically sorts out images. Added navigation options if you want to open up a url inside a webview. Sorts out youtube channels by default. You can see the most recent videos on bookmarked youtube channels. The last five videos. Added an option to open youtube links in a random invidious instance. Added a search bar to search through all your bookmarks and asearch bar for icons. There is a cardview section which is an alternative to using the dropdown. You can choose what bookmarks open when the application is loaded. You can choose what page is loaded in general. Most of the features are in the settings section. The invidious links option parses the invidious instance list. You can be update the instance list by just replaceing the html file with the redownloaded invidious instance list https://redirect.invidious.io/. Save the html page and overwrite the old one. I think the kevinrocks instance is dead. That isn't an error in the application. A few of the instances on the list went down in the last week or so.



-------------------------------------------
Hidden bookmarks
-------------------------------------------
There is a password protected Bookmarks section which can only be accessed by typing @secret or @hidden into the main form(the one with the https:// placeholder). To add new pages to this section, you would type something like https://www.google.com@secret or https://www.google.com@hidden . To just view the section, you would only type @secret or @hidden into the main form. You are also offered the option to change the passphrase. After it has been changed, hidden bookmarks can be added with   password https://www.google.com  . It's just your created password followed by a space and then the url you are adding. To access the hidden bookmarks with the new password, you just type in the password. You don't need the @ symbol if you created a password. You can now move bookmarks from the main section to the password section by editing bookmarks and adding you password before them. Just like you would add a new url to the password section. It sorts out nsfw content into the password protected section based off a file put together by nofap lol. You can change the default behavior by modifying that file. Search engines aren't filtered out by default and imgur is at the moment. You can modify the file to change what sites are filtered.

1)To import your bookmarks, go to the firefox settings button>bookmarks>manage bookmarks>import and backup>click on backup

2)then open that json file in the application's file picker.

3)It will probably take a second. That's the application trying to pull out images and sorting out NSFW content.

If you don't provide information about a website, it will try and scrape the website. Kinda doubt there would be enough requests to cause any problems. Think it's only 1 request per bookmark.

If you try and import your bookmarks a second time, it will only add your newly added bookmarks. You can update the application by importing your firefox bookmarks multiple times. 

-------------------------------------------
Downloads
-------------------------------------------
*The windows application needs to be repackaged with latest updates

windows 
download link= https://icedrive.net/s/g62kVCYYfghSCZbu2fB53tfY7h7A

linux 
download link= https://icedrive.net/s/3WzG9RStYDXxbX58w7P6j9B4ghVw


The android application is hosted on github.
----------------------------------------
I quit working on the android application a while back. Got tired of repackaging it over and over again on a bunch of systems. You can probably still run what i had at the time. If you are curious about pythonforandroid, shows that it can be ported to android. I was a little further along then what is shown there. Also shows why it's taken a while to get an application running. Was going to be a password manager. I also was packaging it on linux, windows, android, as a server and a webview. The application behaves differently between running as webview and a server. Part of this was me plaing around with pywebview. The application uses both the flask pywebview api and the pywebview javascript api. Figured mine as well try out the non flask option. Android was kind of an afterthought.

Todo list
----------------------------------------------

improve how the application scrapes libreddit, fix up the "speeddial" page, continue working on the feedreader, if i decide to add m3u support, it'd probably be through vlc, WORK UP THE NERVE TO PUBLISH THE APPLICATION, clean up the positioning on a few of the pages, look into building a fireefox extension to dynaimically add bookmarks, add libreddit instances as its own button, add a filepicker or a form to update the background images(This is currently only available with the ini file), look into porting the application to mobile(probably with an api and kivy).

----------------------
Some ideas for the future
1)might add m3u support
2)maybe nlp for categories 3) 
3)feedreading stuff.


Try not to go to overboard though.
really need to get things together with version control. I didn't really originally plan on it being as comprehensive as it currently is. Think running it as a server is what makes it a pretty great idea for an application. If anyone has any advice on how I should go about publishing a python application hmu. Kind of shy and not really sure where I should start. I'd like to get it on one of the linux software centers.


