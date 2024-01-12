# YouTube to MP3 & MP4 Developer APIs
If you are a Web Developer and looking for a Video Downloader API for your projects then you are at the right place. We offer super fast iFrame converter APIs to allow you to download videos without using your server resources. Our APIs work with any programming language like PHP, Python, JavaScript, jQuery, Ajax, JSON, Node.JS, Swift, C#, Java, Android, & iOS.

Our API supports video platforms like YouTube. Try our YouTube to MP3 API.

## Single Button API

**GET** `https://apiyt.cc/{FTYPE}/{VIDEO_ID}`

**Parameters:**

**FTYPE:** `mp3` or `mp4`

**VIDEO_ID:** https://www.youtube.com/watch?v= `pRpeEdMmmQ0`

MP3/MP4 iFrame Code:
```
<iframe src="https://apiyt.cc/mp3/pRpeEdMmmQ0" style="width: 160px; height: 60px;" width="100%" height="100%"
allowtransparency="true" scrolling="no" style="border:none"></iframe>
```
**Generates this:**

![MP3 button / Music Download](https://apiyt.cc/assets/images/mp3.png)
![MP4 button / Video Download](https://apiyt.cc/assets/images/mp4.png)


## Widget API

**GET** `https://apiyt.cc/{FTYPE}/{VIDEO_ID}`

**Parameters:**

**FTYPE:** `widget`

**VIDEO_ID:** https://www.youtube.com/watch?v= `pRpeEdMmmQ0`

iFrame Code:
```
<iframe id="buttonApi" src="https://apiyt.cc/widget/pRpeEdMmmQ0" width="100%" height="100%"
allowtransparency="true" scrolling="no" style="border:none;overflow:hidden;height: 300px;width: 100%;"></iframe>

```
Javascript code for automatic (Responsive) resizing:
```
<!-- Put the Library in your <head> tag -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/iframe-resizer/4.3.2/iframeResizer.min.js"></script>

<!-- Put the resizer code after the <iframe> tag -->
<script>iFrameResize({ log: false }, '#widgetApi')</script>
```
**Generates this:**

![Multi buttons / Music and Video Download](https://apiyt.cc/assets/images/widgets.png)

## Search API

**GET** `https://apiyt.cc/{FTYPE}/{QUERY}`

**Parameters:**

**FTYPE:** `search`

**QUERY:** Post Malone

iFrame Code:
```
<iframe id="SearchApi" src="https://apiyt.cc/search/post+malone" width="100%" height="530" allowtransparency="true" style="border:none"></iframe>
```
**Generates this:**

![Search Video](https://apiyt.cc/assets/images/search.png)


**Official API Websites:** https://apiyt.cc/

**Demo:** https://TubeMp3.biz `or` https://TubeMp3.websiteseguro.com

**More demo:** https://youtubeconversor1.websiteseguro.com `or` https://youtubefastmp31.websiteseguro.com/
