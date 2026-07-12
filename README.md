# Moonlight Downloader API Guide

Welcome to the API guide of Moonlight Downloader, an API for downloading images and videos from all across the internet.
Powered by [YT-DLP](https://github.com/yt-dlp/yt-dlp) and Mike Fährmann's [Gallery-DL](https://github.com/mikf/gallery-dl).
<br />

## RECEIVING API KEY
Before using the endpoints, you need an API Key. The only way to obtain a Moonlight Downloader API Key is from its [Telegram Bot]().
Please procceed to get your API Key and then start using the API itself.
<br />

## USAGE
Usage of the API is pretty simple. Usually the workflow would be:
1. First, [getting the meta data](content/getMetaData.md) for your video/image of choice (if needed).
2. Then, [processing](content/processUrl.md) the said URL and feeding the format to the server (the format query, as said in the documentation, is only required if your media of choice is a video)
3. And finally, [requesting](content/requestMediaById.md) the media itself from the server to be streamed.
<br />

> [!NOTE]
> The processing and streaming the actual media from the server was seperated into two different steps, in order for the API to support downloading playlists or posts with multiple videos/images.

<br />

### Enjoy!
