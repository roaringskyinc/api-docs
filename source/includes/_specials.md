# Specials

## Get current specials

```shell
curl -H "Authorization: Bearer {token}" https://kapi.dineoncampus.com/specials
```

> The above command returns JSON structured like this:

```json
{
  "special_offers": [
    {
      "active": true,
      "brief": "This is a brief description of the special.",
      "description": "This is the description of the special.",
      "end": "2022-04-22T17:00:00.000-07:00",
      "id": "61ca15d6b63f1e0e69d5a499",
      "name": "The name of the special",
      "public_on": "2021-12-27T11:36:54.000-08:00",
      "start": "2022-01-18T09:00:00.000-08:00"
    }
  ]
}
```

This endpoint retrieves all current specials.

### HTTP Request

`GET http://kapi.dineoncampus.com/specials`

### Query Parameters

| Parameter | Required | Description                                    |
| --------- | -------- | ---------------------------------------------- |
| site_id   | yes      | The Id of your site should be provided to you. |

<aside class="success">
Request volumes are logged and monitored. Request thresholds will be enforced in the near future 😀.
</aside>