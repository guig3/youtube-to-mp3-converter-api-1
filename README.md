# **YouTube to MP3 API Documentation**

**Base URL**:<br> `https://tube-mp31.p.rapidapi.com/`

## **Endpoints**
Converts a YouTube video to MP3 format and provides a direct download 

**METHOD POST** `https://tube-mp31.p.rapidapi.com/json`<br><br>

## **Request**<br>

###  Headers

```
{
  "Content-Type": "application/json"
}
```

###  Body Parameters<br>
<table>
    <thead>
        <tr>
            <th>Parameter</th>
            <th>Type</th>
            <th>Required</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>videoId</td>
            <td>string</td>
            <td>Yes</td>
            <td>The YouTube video ID to be converted.</td>
        </tr>
    </tbody>
</table>

### Example Request Body

```
{
  "videoId": "K4xl1T_lyiM"
}
```



<br>

##  **Response**

### Success Response<br>
<table>
    <thead>
        <tr>
            <th>Field</th>
            <th>Type</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>status</td>
            <td>string</td>
            <td>Status of the request (success).</td>
        </tr>
        <tr>
            <td>response</td>
            <td>string</td>
            <td>Direct download URL for the converted MP3.</td>
        </tr>
    </tbody>
</table>

- **Example Success Response**<br>

```
{
  "status": "success",
  "result": [
    {
      "videoId": "Video ID",
      "title": "Artist - Song Name",
      "author": "Author",
      "duration": 167,
      "dlurl": "https://example.com/downloads/audio.mp3",
      "token": "JTdCJTIyaWQlMjIlM0ElMjIxa0FudTdWaXI...."
    }
  ]
}
```
<br>

### Error Responses<br>
<table>
    <thead>
        <tr>
            <th>Response</th>
            <th>Field</th>
            <th>Type</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Error Response</td>
            <td>error</td>
            <td>string</td>
            <td>Error message if the request fails.</td>
        </tr>
    </tbody>
</table>

- **Example Error Response (Missing videoId)**<br>

```
{
  "error": "\"videoId\" parameter is mandatory."
}
```

- **Example Error Response (Method Not Allowed)**<br>

```
{
  "error": "Method not permitted."
}
```

<br>

-----------

### **Rate Limiting**

- **Request Limit**: 100 requests per minute.
- **Status Code:** 429 Too Many Requests is returned when the limit is exceeded.


-----------

### **Error Handling**

- 400 Bad Request: Returned if the videoId parameter is missing or invalid.
- 405 Method Not Allowed: Returned if a method other than POST is used.
- 500 Internal Server Error: Indicates a server-side issue.


-----------

### **Features**
- Converts YouTube videos to MP3 format effortlessly.
- Provides direct download links for easy integration.
- Supports high-quality audio conversion.


-----------

### **Contact and Support**
For assistance, feel free to reach out to our support team at support@tubemp3.net.

Enjoy building with the **YouTube to MP3 API**! 🚀

<p>
<a href="https://apiyt.cc" target="_blank">https://apiyt.cc</a> or <a href="https://TubeMp3.net" target="_blank">https://TubeMp3.net</a>
</p>
