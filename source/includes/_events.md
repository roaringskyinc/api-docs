# Events

## Get upcoming events

```shell
curl -H "Authorization: Bearer {token}" https://kapi.dineoncampus.com/events/upcoming
```

> The above command returns JSON structured like this:

```json
{
  "current_events": [
    {
      "active": true,
      "description": "Looking to learn more about Superfood Tomato?\nMake sure to stop by Jasper Kane Café from\n1PM – 2PM to learn more about the nutritional\nbenefits of Tomatoes.",
      "end": "2019-07-09T11:00:00.000-07:00",
      "featured": null,
      "id": "5d13d84e4198d409c39c8056",
      "picture": null,
      "start": "2019-07-09T10:00:00.000-07:00",
      "title": "Superfood Tabling at Jasper Kane Café"
    },
    {
      "active": true,
      "description": "Locally grown produce and freshly prepared\nbakery items will be available at The\nMarketplace at Kimmel from 11AM – 2PM!\nDon’t miss out on supporting some of our\namazing local farmers & tasting their delicious\nproduce!",
      "end": "2019-07-11T11:00:00.000-07:00",
      "featured": null,
      "id": "5d13d8774198d409c39c9158",
      "picture": null,
      "start": "2019-07-11T08:00:00.000-07:00",
      "title": "Farmers Market at The Marketplace at Kimmel"
    },
    {
      "active": true,
      "description": "We’re tossing up something special at the\nNYU Eats at Downstein for dinner on\nMonday night. Make sure to stop by to create\nyour own wings.",
      "end": "2019-07-15T17:00:00.000-07:00",
      "featured": null,
      "id": "5d13d8bf4198d409c39c9174",
      "picture": null,
      "start": "2019-07-15T14:00:00.000-07:00",
      "title": "Wing Day at NYU Eats at Downstein"
    },
    {
      "active": true,
      "description": "Looking to learn more about Superfood Tomato?\nMake sure to stop by The Marketplace at\nKimmel from 1PM – 2PM to learn more about the\nnutritional benefits of Tomatoes with RD\nChristina.",
      "end": "2019-07-16T11:00:00.000-07:00",
      "featured": null,
      "id": "5d13d8f14198d409c39c9181",
      "picture": null,
      "start": "2019-07-16T10:00:00.000-07:00",
      "title": "Superfood Tabling at The Marketplace at Kimmel"
    }
  ],
  "event_slug": "events",
  "status": "success"
}
```

This endpoint retrieves all upcoming events.

### HTTP Request

`GET https://kapi.dineoncampus.com/events/upcoming`

### Query Parameters

| Parameter | Required | Description                                    |
| --------- | -------- | ---------------------------------------------- |
| site_id   | yes      | The Id of your site should be provided to you. |

<aside class="success">
Request volumes are logged and monitored. Request thresholds will be enforced in the near future 😀.
</aside>
