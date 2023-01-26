# Bookmarklet-to-get-YouTube-channel-ID
Bookmarklet to get YouTube channel ID

Copy the following code and create a new favorite/bookmark with the code pasted into the url textbox. You can name the favorite/bookmark whatever you want since it will not affect the script.
Now when you are on the main page of a YouTube channel, you can click on the favorite/bookmark you created and it will show a the base channel ID URL and the URL to a playlist with all of the public videos on the channel.
```
javascript:let baseChannelIdUrl=document.querySelector("meta[property='og:url']").getAttribute("content"),channelUploadsUrl=baseChannelIdUrl.replace("https://www.youtube.com/channel/", "https://www.youtube.com/playlist?list=").replace("UC", "UU");alert("Base Channel ID URL:\n" + baseChannelIdUrl + "\nChannel Uploads URL:\n" + channelUploadsUrl);void(0);
```
