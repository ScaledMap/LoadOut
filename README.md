recent update
-------------
june 21:Added a default category called devenv. Think it's a cool idea for a default category. Has jsfiddle, bash, python repls running in the browser. Fixed a bug in the cardview where cards wouldn't propegate properly if the title was too long. Added a hash to unfilter values. if you want to hide a value fromt the filters, type @hide in the description. I made it so bookmarks added from the webview get added to a category called webview. Good way to keep stumbleupon bookmarks seperate. That website will kind of dramatically increase how many bookmarks you have lol.

Found the drive i was packaging the windows application on. My windows boot is borked. reinstalling. Should be able to get that working though. I guess some random update broke the install. Plan on updating the windows version in the next update. It hasn't been updated in a really, really long time.

june 15:

Added forms to customize background images. Backgrounds are set as a mate walpaper at the moment. Clicking restore to default will revert to the old background images. Setting the color will set background images to None. No longer have to customize things from the ini file. You will probably need to add custom background images to the static folder. They should also be fairly big images. 

paginated the youtube videos. will pull out /channels/ /c/ and /user/ urls and put them in the channel section. You might need to reload things if it doesnt pull the videos out of the channels. Same with the redirects to invidious and reddit. To update the application, you can just overwrite the old database file. Thats how i usually do things.  Invidious is working better now. Decided to parse the json file instead of the html file. Probably going to make a json file for libredit eventually. It's a better way to do things.

crap... forgot to fix the typo again lol...

Hosting the file on icedrive until i publish it

basic usage:
----------------
 I usually do pretty much everything on the web at point. This type if thing works great for how i use computers

open image in new tab/open image link/ to save images. its usually better to pull images out of websites directly. googles images, and bing images, etc. are a work in progress.

looks for filetype e.g .jpeg, .gif, or some search engine proxies work. Should support any filetype listed on firefox's documentation.

youtube.com/watch = to filter iframes and construct playlists out of categories(great for creating music playlists)

/channel/, /c/, /user/ = to pull out the bookmarked channel videos

it can pull these out of your bookmarks or you can just add them directly to the application and sort them yourself


@secret/@hidden == default passwords

you can add anything you want but those urls will be sorted into the appropriate categories by default. so yeah... Kind of gives your bookmarks more utility. 

Title


-------
Loadout
-------

LoadOut is a Bookmark manager I've been working on to help manage and organize my bookmarks. It's a Pywebview application built on flask. You can run it as a server or as a webview.  It allows you to import your bookmarks from firefox and create categories to interact with those bookmarks. It would also probably be useful for situations where you want to avoid messing with the keyboard. There was a time where i was using opera because speeddial was useful. I'd kind of like it to be a more flexible alternative to something like pocket or speedial. Works across browsers at least. My advice would be to run it as a server. You can set loadout to boot at startup and make it your homepage.  Another option would be to change the icon(so it looks like firefox or whatever your default browser is) and run it as a server. it will try and open your default browser when you click on the exe.

You could also use this with librewolf or an alternative browser. Some of the more privacy focused browsers don't do cookies by default. This would be really useful with something like librewolf.

You could also use the webview as a browser. Kind of a limiting experience but you could try it. Pywebview doesn't default to persistent cookies. History won't show up when you open links in the webview. Stumbleupon(guess its "cloudhiker now... lol lost the domain") works well in the webview. You can add bookmarks through the webview like you normally would in the browser. Works well if you want to keep stumbleupon stuff seperate from normal bookmarks.


-------------------------------------------
Downloads
-------------------------------------------
*The windows application needs to be repackaged with latest updates

windows 
download link= https://icedrive.net/s/g62kVCYYfghSCZbu2fB53tfY7h7A

linux 
download link= https://icedrive.net/s/B64v9wB9w9NygQah4Xu2A3i1B6uz



-------
features/
-------
atomatically sorts out images. Added navigation options if you want to open up a url inside a webview. Sorts out youtube channels by default. You can see the most recent videos on bookmarked youtube channels. Added an option to open youtube links in a random invidious instance or libreddit instance. Added a search bar to search through all your bookmarks and a search bar for icons. There is a cardview section which is an alternative to using the dropdown(noscript will break the dropdown). Can color code categories. You can choose what bookmarks open when the application is loaded. You can choose what page is loaded in general. Most of the features are in the settings section. Customizeable backgrounds. The invidious links option parses the github .json file. You can be update the instance list by just replaceing the json file with the redownloaded json list https://api.invidious.io/. It's saved as instances.json in the static folder. I think the kevinrocks instance is dead. That isn't an error in the application. A few of the instances on the list went down in the last week or so.



-------------------------------------------
Hidden bookmarks
-------------------------------------------
There is a password protected Bookmarks section which can only be accessed by typing @secret or @hidden into the main form(the one with the https:// placeholder). To add new pages to this section, you would type something like https://www.google.com@secret or https://www.google.com@hidden . To just view the section, you would only type @secret or @hidden into the main form. You are also offered the option to change the passphrase. After it has been changed, hidden bookmarks can be added with   password https://www.google.com  . It's just your created password followed by a space and then the url you are adding. To access the hidden bookmarks with the new password, you just type in the password. You don't need the @ symbol if you created a password. You can now move bookmarks from the main section to the password section by editing bookmarks and adding you password before them. Just like you would add a new url to the password section. It sorts out nsfw content into the password protected section based off a file put together by nofap lol. You can change the default behavior by modifying that file. Search engines aren't filtered out by default and imgur is at the moment. You can modify the file to change what sites are filtered.

1)To import your bookmarks, go to the firefox settings button>bookmarks>manage bookmarks>import and backup>click on backup

2)then open that json file in the application's file picker.

3)It will probably take a second. That's the application trying to pull out images and sorting out NSFW content.

If you don't provide information about a website, it will try and scrape the website. Kinda doubt there would be enough requests to cause any problems. Think it's only 1 request per bookmark.

If you try and import your bookmarks a second time, it will only add your newly added bookmarks. You can update the application by importing your firefox bookmarks multiple times. 




The android application is hosted on github.
----------------------------------------
I quit working on the android application a while back. Got tired of repackaging it over and over again on a bunch of systems. You can probably still run what i had at the time. If you are curious about pythonforandroid, shows that it can be ported to android. I was a little further along then what is shown there. Also shows why it's taken a while to get an application running. Was going to be a password manager. I also was packaging it on linux, windows, android, as a server and a webview. The application behaves differently between running as webview and a server. Part of this was me plaing around with pywebview. The application uses both the flask pywebview api and the pywebview javascript api. Figured mine as well try out the non flask option. Android was kind of an afterthought.

Todo list
----------------------------------------------
Paginate the extracted youtube videos, update instance lists, fix redirect from the index to libreddit and invidious, export bookmarks button. Add filters for search engine proxies. I usually do pretty much everything on the web at point. This type if thing works great for how i use computers.



