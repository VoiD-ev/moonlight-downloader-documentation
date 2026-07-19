# Request Media by ID

### Endpoint
```
GET /media/{id}
```

## PARAMETERS

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
![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) 401 - Unauthorized <br />
![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) 404 - Not Found <br />
![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) 429 - Too Many Requests <br />
<br />

## RESPONSE EXAMPLE
> [!IMPORTANT]
> If the operation is successful, the response wouldn't be in JSON format. <br />
> Instead, the media will be streamed directly.
<br />

```json
{
  "success": false,
  "error": "This file doesn't exist on the server.",
  "code": 404,
  "results": []
}
```
