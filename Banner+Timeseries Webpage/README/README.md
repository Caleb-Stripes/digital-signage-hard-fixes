This documentation should guide you in an effort to create a timeseries with a banner for CommunityHub Digital Signage.

Currently 2021.07.01 the version of Communityhub Digital Signage in use by the Environmental Dashboard project uses web URLs to create carousels for running in displays on Digital Signage running the Communityhub Software called media-player. Thus in order for timeseries with banner assets created in this way to be used by that software they will have to be accessible via web browsers.
Steps to create your content are listed below.

1) Between the <head> </head> tags , there is a lineof code “<meta name=”description”content=...”. Replace this content with a suitabledescription which reflects what time series theweb page will be displaying.

2) Similarly, change the title for the web page betweenthe <title> </title> tags.

3) The webpages we are currently making function byembedding other websites/slideshowsthat have already been made through iframes. Therefore,we will need to have access to theURL of the websites that have already been made.

4) The banner we are using is a slideshow that willbe played on our web page. To get a URLlink to this, go to the presentation on google slides.Click “File”, and then “Publish to Web”. Clickon “Embed”, and check the options “Start slideshowas soon as the player loads” & “Restart theslideshow after the first slide”.

5) Copy the portion of the link similar to the oneshown in the image above and replace this linkwith the link already present in the first “<iframesrc tag.” in the HTML code file. This isn’t thefinal link we will use. You will have to add “&rm=minimal”to the end of the link to ensure that thegoogle slides navigation system doesn’t appear inour webpage.

6) To get the URL link for the banner, go to thislink:“https://environmentaldashboard.org/chart/index.php”and select the wanted meter, and selectany other wanted options like “Title image”, and “TitleText”. Once you submit,you will beredirected to the webpage with the time series. You will find the URL in the chrome address bar.This isn’t the final URL we are going to use. You will need to add “&hide_navbar=true”,“&hide_menu=true” to the end of the URL.
There are other parameters that can be added to the end of the URL to edit our time series appearance. More information on that can be found on this link:
“https://www.notion.so/Setting-Up-a-Time-Series-Graph-b9619065ded24ca2aac0d71acf43346a”7)Now that we have the URL for the time series, youcan go ahead and replace the linkcurrently present in the second iframe src tag. Once the code is saved, and the tab displayingthe webpage refreshed, it should show the new webpage with the changes made.
