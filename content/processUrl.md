# Process URL

### Endpoint
```
GET /process
```

## PARAMETERS

### Query Parameters
<html>
<table> 
<tbody>
  <tr>
    <th>url *</th>
    <td>A string representing the url of the media you want to download.</td>
  </tr>
  <tr>
    <th>format</th>
    <td>
      A string representing the quality, format and other traits of a video.<br />
      If left empty, the media would be defaulted to image.
    </td>
  </tr>
</tbody>
</table>
<br />
</html>

### Body Parameters
<html>
  <table>
    <tbody>
      <tr>
        <th>Authorization *</th>
        <td>
          A long string of characters representing your API Key.<br />
          Mind that the server expects the key to be sent as a bearer token.
        </td>
      </tr>
    </tbody>
  </table>
  <br />
</html>

> A (*) sign indicates required parameters
<br />

## RESPONSES
![#00ff00](https://placehold.co/15x15/00ff00/00ff00.png) 201 - Created <br />
![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) 400 - Bad Request <br />
![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) 401 - Unauthorized <br />
![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) 403 - Forbidden (file exceeded server memory) <br />
![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) 422 - Unprocessable Content <br />
![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) 429 - Too Many Requests <br />
<br />

## RESPONSE EXAMPLE
```json
{
  "success": true,
  "error": null,
  "code": 200,
  "results": [
    {
        "id": "xc8XRl-6V68",
        "url": "https://api.moonlight-downloader.ir/media/xc8XRl-6V68",
        "type": "mp4"
    },
    {
        "id": "DaqHYGTR7qB",
        "url": "https://api.moonlight-downloader.ir/media/DaqHYGTR7qB",
        "type": "png"
    }
  ]
}
```
