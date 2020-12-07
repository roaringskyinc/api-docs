# Locations

## Get open locations

```shell
curl -H "Authorization: Bearer {token}" https://kapi.dineoncampus.com/locations/open
```

> The above command returns JSON structured like this:

```json
{
  "location_schedules": [
    {
      "_type": "DOC::WebtritionLocation",
      "id": "5b8030be1178e90bcf85640b",
      "name": "Business Perks",
      "schedules": [
        {
          "created_at": "2019-01-11T07:02:36.531-08:00",
          "days": [1, 2, 3, 4],
          "end": "2019-05-07T15:00:19.000-07:00",
          "end_hour": 18,
          "end_minutes": 0,
          "id": "5c38b00cbddf43091fa890bf",
          "open_late": false,
          "start": "2019-01-14T04:00:19.000-08:00",
          "start_hour": 8,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-01-11T07:02:47.823-08:00",
          "days": [5],
          "end": "2019-05-03T10:00:37.000-07:00",
          "end_hour": 13,
          "end_minutes": 0,
          "id": "5c38b017bddf43090b799e51",
          "open_late": false,
          "start": "2019-01-18T04:00:37.000-08:00",
          "start_hour": 8,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-05-01T12:56:51.732-07:00",
          "days": [3],
          "end": "2019-05-08T14:00:37.000-07:00",
          "end_hour": 17,
          "end_minutes": 0,
          "id": "5cc9fa031ca48e0e6f7cb372",
          "open_late": false,
          "start": "2019-05-08T05:00:37.000-07:00",
          "start_hour": 8,
          "start_minutes": 0,
          "type": "location"
        }
      ],
      "sort_order": 2,
      "type": null,
      "webtrition_version": 2
    }
  ],
  "records": 13,
  "request_time": 0.903337163,
  "status": "success"
}
```

This endpoint retrieves current, open locations.

### HTTP Request

`GET http://kapi.dineoncampus.com/locations/open`

### Query Parameters

| Parameter | Required | Description                           |
| --------- | -------- | ------------------------------------- |
| site_id   | yes      | The Id of your site, provided to you. |
| timestamp | yes      | Formatted as YYYY-MM-DD               |

## Get location details

```shell
curl -H "Authorization: Bearer {token}" https://kapi.dineoncampus.com/location/info
```

> The above command returns JSON structured like this:

```json
{
  "location": {
    "address": {
      "city": "Anytown",
      "coordinates": [
        -118.911467,
        34.84084
      ],
      "state": "California",
      "street": "123 Anystreet",
      "zip_code": "90001"
    },
    "building": {
      "id": "5d7712054198d40e5d6b123z",
      "name": "Building A"
    },
    "id": "5d52e7a44198d409cf40h762",
    "name": "Starbucks"
  },
  "records": 1,
  "request_time": 0.018607338,
  "status": "success"
}
```

This endpoint retrieves details of a single location.

### HTTP Request

`GET http://kapi.dineoncampus.com/location/info`

### Query Parameters

| Parameter   | Required | Description             |
| ----------- | -------- | ----------------------- |
| location_id | yes      | The Id of the location. |

## Get the status of all locations

```shell
curl -H "Authorization: Bearer {token}" https://kapi.dineoncampus.com/locations/status
```

> The above command returns JSON structured like this:

```json
{
    "locations": [
        {
            "id": "5d52e7a44198d409cf40f18b",
            "name": "Location Name",
            "open": true,
            "address": {
                "id": "5d545dbe4829d40b9fdfsdfe",
                "street": "123 Any Street",
                "metadata": null,
                "city": "Anytown",
                "state": "California",
                "zip_code": "90210",
                "lat": 34.673088615115525,
                "lon": -113.76468008756638,
                "phone": null,
                "dst": false,
                "gmt": 0,
                "phone_formatted": null,
                "ext_formatted": null,
                "gmt_offset": 0,
                "coordinates": [
                    -113.6531377,
                    34.6715395
                ],
                "manual_coords": [
                    34.673088615115525,
                    -113.76468008756638
                ],
                "abbreviation": null,
                "zone_name": null
            }
        }
    ]
}
```

This endpoint retrieves the status and address of all locations.

### HTTP Request

`GET http://kapi.dineoncampus.com/locations/status`

### Query Parameters

| Parameter | Required | Description                           |
| --------- | -------- | ------------------------------------- |
| site_id   | yes      | The Id of your site, provided to you. |

<aside class="success">
Request volumes are logged and monitored. Request thresholds will be enforced in the near future 😀.
</aside>
