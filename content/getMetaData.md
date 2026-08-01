# Get Meta Data

### Endpoint
```
GET /meta
```

## PARAMETERS

### Query Parameters
<html>
<table> 
<tbody>
  <tr>
    <th>url *</th>
    <td>A string representing the url of the media you want to get the meta data for.</td>
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
![#00ff00](https://placehold.co/15x15/00ff00/00ff00.png) 200 - OK <br />
![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) 400 - Bad Request <br />
![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) 401 - Unauthorized <br />
![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) 422 - Unprocessable Content <br />
![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) 429 - Too Many Requests <br />
<br />

## RESPONSE EXAMPLE
> [!NOTE]
> Entries are empty as long as the requested metadata is not a playlist.
> However if the requested metadata IS a playlist, the result will be the metadata of the playlist itself and the entries will be filled in with the metadata of the individual videos.
<br />

```json
{
  "success": true,
  "error": null,
  "code": 200,
  "results": [
    {
      "id": "AseTNgPRDH8",
      "thumbnail": "https://example-site.com/path/to/thumbnail/thumbnail-image.png",
      "title": "This amazing video will warm your heart!",
      "description": "hello! today i'm going to show you the most awesome video ever! follow for more...",
      "formats": [
        {
          "id": 137,
          "info": "720p",
          "width": 1280,
          "height": 720,
          "audio-channels": 1
        },
        {
          "id": 138,
          "info": "1080p",
          "width": 1920,
          "height": 1080,
          "audio-channels": 1
        }
      ],
      "entries": []
    }
  ]
}
```
