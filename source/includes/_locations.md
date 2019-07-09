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
          "days": [
            1,
            2,
            3,
            4
          ],
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
          "days": [
            5
          ],
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
          "days": [
            3
          ],
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
    },
    {
      "_type": "DOC::ConceptLocation",
      "id": "587655acee596f59b1adbe6c",
      "name": "Chili's Grill & Bar",
      "schedules": [
        {
          "created_at": "2019-01-11T07:01:02.418-08:00",
          "days": [
            0
          ],
          "end": "2019-05-05T20:00:43.000-07:00",
          "end_hour": 23,
          "end_minutes": 0,
          "id": "5c38afaebddf4309161e50c5",
          "open_late": false,
          "start": "2019-01-13T11:00:43.000-08:00",
          "start_hour": 15,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-01-11T07:01:24.504-08:00",
          "days": [
            1,
            2,
            3,
            4
          ],
          "end": "2019-08-02T13:00:06.000-07:00",
          "end_hour": 16,
          "end_minutes": 0,
          "id": "5c38afc4bddf43090b7980dd",
          "open_late": false,
          "start": "2019-01-14T07:00:06.000-08:00",
          "start_hour": 11,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-01-11T07:01:51.442-08:00",
          "days": [
            5
          ],
          "end": "2019-08-02T12:00:25.000-07:00",
          "end_hour": 15,
          "end_minutes": 0,
          "id": "5c38afdfbddf4309161e510f",
          "open_late": false,
          "start": "2019-01-18T07:00:25.000-08:00",
          "start_hour": 11,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-01-11T07:02:10.098-08:00",
          "days": [
            6
          ],
          "end": "2019-05-04T19:00:52.000-07:00",
          "end_hour": 22,
          "end_minutes": 0,
          "id": "5c38aff2bddf43090b799052",
          "open_late": false,
          "start": "2019-01-19T11:00:52.000-08:00",
          "start_hour": 15,
          "start_minutes": 0,
          "type": "location"
        }
      ],
      "sort_order": 3,
      "type": "concept",
      "webtrition_version": 2
    },
    {
      "_type": "DOC::ConceptLocation",
      "id": "587655abee596f59b1adbe64",
      "name": "Chop'd & Wrap'd",
      "schedules": [
        {
          "created_at": "2019-01-11T07:00:13.992-08:00",
          "days": [
            1,
            2,
            3,
            4
          ],
          "end": "2019-05-08T12:00:01.000-07:00",
          "end_hour": 15,
          "end_minutes": 0,
          "id": "5c38af7dbddf43090b7968cf",
          "open_late": false,
          "start": "2019-01-14T06:00:01.000-08:00",
          "start_hour": 10,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-01-11T07:00:37.727-08:00",
          "days": [
            5
          ],
          "end": "2019-05-03T10:00:21.000-07:00",
          "end_hour": 13,
          "end_minutes": 0,
          "id": "5c38af95bddf43092878d52b",
          "open_late": false,
          "start": "2019-01-18T06:00:21.000-08:00",
          "start_hour": 10,
          "start_minutes": 0,
          "type": "location"
        }
      ],
      "sort_order": 4,
      "type": "concept",
      "webtrition_version": 2
    },
    {
      "_type": "DOC::ConceptLocation",
      "id": "5b4f4e81f3eeb609aaec14b6",
      "name": "Elements Bistro",
      "schedules": [
        {
          "created_at": "2019-01-11T06:58:51.493-08:00",
          "days": [
            1,
            2,
            3,
            4
          ],
          "end": "2019-08-02T13:00:40.000-07:00",
          "end_hour": 16,
          "end_minutes": 0,
          "id": "5c38af2bbddf43090b7934cc",
          "open_late": false,
          "start": "2019-01-14T07:00:40.000-08:00",
          "start_hour": 11,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-05-13T09:42:33.906-07:00",
          "days": [
            5
          ],
          "end": "2019-08-02T12:00:24.000-07:00",
          "end_hour": 15,
          "end_minutes": 0,
          "id": "5cd99e794198d40838c2824b",
          "open_late": false,
          "start": "2019-05-13T08:00:24.000-07:00",
          "start_hour": 11,
          "start_minutes": 0,
          "type": "location"
        }
      ],
      "sort_order": 5,
      "type": "concept",
      "webtrition_version": 2
    },
    {
      "_type": "DOC::ConceptLocation",
      "id": "587655acee596f59b1adbe68",
      "name": "Fenn Shoppe",
      "schedules": [
        {
          "created_at": "2019-01-11T06:58:10.666-08:00",
          "days": [
            1,
            2,
            3,
            4
          ],
          "end": "2019-05-02T19:00:37.000-07:00",
          "end_hour": 22,
          "end_minutes": 0,
          "id": "5c38af02bddf4309161e36d9",
          "open_late": false,
          "start": "2019-01-14T03:30:37.000-08:00",
          "start_hour": 7,
          "start_minutes": 30,
          "type": "location"
        },
        {
          "created_at": "2019-01-11T06:58:34.751-08:00",
          "days": [
            5
          ],
          "end": "2019-05-10T13:00:18.000-07:00",
          "end_hour": 16,
          "end_minutes": 0,
          "id": "5c38af1abddf43090b7934ca",
          "open_late": false,
          "start": "2019-01-18T03:30:18.000-08:00",
          "start_hour": 7,
          "start_minutes": 30,
          "type": "location"
        },
        {
          "created_at": "2019-05-01T12:58:14.000-07:00",
          "days": [
            1,
            2,
            3
          ],
          "end": "2019-05-08T21:00:50.000-07:00",
          "end_hour": 0,
          "end_minutes": 0,
          "id": "5cc9fa551ca48e0e5b7d6dbb",
          "open_late": true,
          "start": "2019-05-06T04:30:50.000-07:00",
          "start_hour": 7,
          "start_minutes": 30,
          "type": "location"
        },
        {
          "created_at": "2019-05-01T12:58:42.813-07:00",
          "days": [
            4
          ],
          "end": "2019-05-09T16:00:26.000-07:00",
          "end_hour": 19,
          "end_minutes": 0,
          "id": "5cc9fa721ca48e0e6f7cda3f",
          "open_late": false,
          "start": "2019-05-09T04:30:26.000-07:00",
          "start_hour": 7,
          "start_minutes": 30,
          "type": "location"
        },
        {
          "created_at": "2019-05-01T12:58:59.428-07:00",
          "days": [
            0,
            6
          ],
          "end": "2019-05-05T14:00:49.000-07:00",
          "end_hour": 17,
          "end_minutes": 0,
          "id": "5cc9fa831ca48e0e7a7c9d8b",
          "open_late": false,
          "start": "2019-05-04T05:00:49.000-07:00",
          "start_hour": 8,
          "start_minutes": 0,
          "type": "location"
        }
      ],
      "sort_order": 6,
      "type": "concept",
      "webtrition_version": 2
    },
    {
      "_type": "DOC::WebtritionLocation",
      "id": "587655abee596f59b1adbe63",
      "name": "Grillnation",
      "schedules": [
        {
          "created_at": "2019-01-11T06:57:00.935-08:00",
          "days": [
            1,
            2,
            3,
            4
          ],
          "end": "2019-05-08T14:00:48.000-07:00",
          "end_hour": 17,
          "end_minutes": 0,
          "id": "5c38aebcbddf43090b790b3d",
          "open_late": false,
          "start": "2019-01-14T06:00:48.000-08:00",
          "start_hour": 10,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-01-11T06:57:15.098-08:00",
          "days": [
            5
          ],
          "end": "2019-05-10T11:00:01.000-07:00",
          "end_hour": 14,
          "end_minutes": 0,
          "id": "5c38aecbbddf43090b790bdc",
          "open_late": false,
          "start": "2019-01-18T06:00:01.000-08:00",
          "start_hour": 10,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-05-01T12:47:27.819-07:00",
          "days": [
            4
          ],
          "end": "2019-05-09T12:00:12.000-07:00",
          "end_hour": 15,
          "end_minutes": 0,
          "id": "5cc9f7cf4198d409709e7ea0",
          "open_late": false,
          "start": "2019-05-09T07:00:12.000-07:00",
          "start_hour": 10,
          "start_minutes": 0,
          "type": "location"
        }
      ],
      "sort_order": 7,
      "type": "menubuilder",
      "webtrition_version": 2
    },
    {
      "_type": "DOC::ConceptLocation",
      "id": "5b4f4cf3f3eeb609aaebe67a",
      "name": "HISSHO",
      "schedules": [
        {
          "created_at": "2019-01-11T06:56:31.426-08:00",
          "days": [
            1,
            2,
            3,
            4
          ],
          "end": "2019-05-08T11:00:06.000-07:00",
          "end_hour": 14,
          "end_minutes": 0,
          "id": "5c38ae9fbddf43090b78eecf",
          "open_late": false,
          "start": "2019-01-14T06:30:06.000-08:00",
          "start_hour": 10,
          "start_minutes": 30,
          "type": "location"
        },
        {
          "created_at": "2019-01-11T06:56:43.637-08:00",
          "days": [
            5
          ],
          "end": "2019-05-03T10:00:33.000-07:00",
          "end_hour": 13,
          "end_minutes": 0,
          "id": "5c38aeabbddf43090b78fe92",
          "open_late": false,
          "start": "2019-01-18T06:30:33.000-08:00",
          "start_hour": 10,
          "start_minutes": 30,
          "type": "location"
        }
      ],
      "sort_order": 8,
      "type": "concept",
      "webtrition_version": 2
    },
    {
      "_type": "DOC::WebtritionLocation",
      "id": "587655abee596f59b1adbe65",
      "name": "Outtakes",
      "schedules": [
        {
          "created_at": "2019-01-11T06:53:54.119-08:00",
          "days": [
            1,
            2,
            3,
            4
          ],
          "end": "2019-08-02T12:00:34.000-07:00",
          "end_hour": 15,
          "end_minutes": 0,
          "id": "5c38ae02bddf43091fa87552",
          "open_late": false,
          "start": "2019-01-14T05:00:34.000-08:00",
          "start_hour": 9,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-01-11T06:54:12.588-08:00",
          "days": [
            5
          ],
          "end": "2019-08-02T10:00:55.000-07:00",
          "end_hour": 13,
          "end_minutes": 0,
          "id": "5c38ae14bddf4309161e25a1",
          "open_late": false,
          "start": "2019-01-18T05:00:55.000-08:00",
          "start_hour": 9,
          "start_minutes": 0,
          "type": "location"
        }
      ],
      "sort_order": 10,
      "type": null,
      "webtrition_version": 2
    },
    {
      "_type": "DOC::ConceptLocation",
      "id": "587655acee596f59b1adbe66",
      "name": "Papa John's",
      "schedules": [
        {
          "created_at": "2019-01-11T06:52:58.074-08:00",
          "days": [
            1,
            2,
            3,
            4
          ],
          "end": "2019-05-07T15:00:50.000-07:00",
          "end_hour": 18,
          "end_minutes": 0,
          "id": "5c38adcabddf4309161e1475",
          "open_late": false,
          "start": "2019-01-14T06:00:50.000-08:00",
          "start_hour": 10,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-01-11T06:53:13.478-08:00",
          "days": [
            5
          ],
          "end": "2019-05-10T11:00:59.000-07:00",
          "end_hour": 14,
          "end_minutes": 0,
          "id": "5c38add9bddf43090b7864a2",
          "open_late": false,
          "start": "2019-01-18T06:00:59.000-08:00",
          "start_hour": 10,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-05-01T13:02:05.164-07:00",
          "days": [
            3
          ],
          "end": "2019-05-08T14:00:41.000-07:00",
          "end_hour": 17,
          "end_minutes": 0,
          "id": "5cc9fb3d1ca48e0e647dfeeb",
          "open_late": false,
          "start": "2019-05-08T07:00:41.000-07:00",
          "start_hour": 10,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-05-01T13:02:15.393-07:00",
          "days": [
            4
          ],
          "end": "2019-05-09T13:00:06.000-07:00",
          "end_hour": 16,
          "end_minutes": 0,
          "id": "5cc9fb471ca48e0e5b7e8dea",
          "open_late": false,
          "start": "2019-05-09T07:00:06.000-07:00",
          "start_hour": 10,
          "start_minutes": 0,
          "type": "location"
        }
      ],
      "sort_order": 11,
      "type": "concept",
      "webtrition_version": 2
    },
    {
      "_type": "DOC::WebtritionLocation",
      "id": "587655acee596f59b1adbe6a",
      "name": "The Link",
      "schedules": [
        {
          "created_at": "2019-01-11T06:52:32.390-08:00",
          "days": [
            1,
            2,
            3,
            4
          ],
          "end": "2019-05-03T15:00:08.000-07:00",
          "end_hour": 18,
          "end_minutes": 0,
          "id": "5c38adb0bddf43090b78556b",
          "open_late": false,
          "start": "2019-01-14T04:00:08.000-08:00",
          "start_hour": 8,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-01-11T06:52:44.824-08:00",
          "days": [
            5
          ],
          "end": "2019-05-10T10:00:33.000-07:00",
          "end_hour": 13,
          "end_minutes": 0,
          "id": "5c38adbcbddf43090b78556c",
          "open_late": false,
          "start": "2019-01-18T04:00:33.000-08:00",
          "start_hour": 8,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-05-01T13:00:11.930-07:00",
          "days": [
            1,
            2,
            3
          ],
          "end": "2019-05-08T13:00:56.000-07:00",
          "end_hour": 16,
          "end_minutes": 0,
          "id": "5cc9facb1ca48e0e647db76b",
          "open_late": false,
          "start": "2019-05-06T05:00:56.000-07:00",
          "start_hour": 8,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-05-01T13:00:24.968-07:00",
          "days": [
            4
          ],
          "end": "2019-05-09T12:00:12.000-07:00",
          "end_hour": 15,
          "end_minutes": 0,
          "id": "5cc9fad81ca48e0e7a7ca513",
          "open_late": false,
          "start": "2019-05-09T05:00:12.000-07:00",
          "start_hour": 8,
          "start_minutes": 0,
          "type": "location"
        }
      ],
      "sort_order": 12,
      "type": null,
      "webtrition_version": 2
    },
    {
      "_type": "DOC::WebtritionLocation",
      "id": "587655acee596f59b1adbe67",
      "name": "The Strip",
      "schedules": [
        {
          "created_at": "2019-01-11T06:51:40.808-08:00",
          "days": [
            1,
            2,
            3,
            4
          ],
          "end": "2019-05-07T15:00:07.000-07:00",
          "end_hour": 18,
          "end_minutes": 0,
          "id": "5c38ad7cbddf43090b78415a",
          "open_late": false,
          "start": "2019-01-14T06:00:07.000-08:00",
          "start_hour": 10,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-01-11T06:51:57.131-08:00",
          "days": [
            5
          ],
          "end": "2019-05-10T11:00:42.000-07:00",
          "end_hour": 14,
          "end_minutes": 0,
          "id": "5c38ad8dbddf43090b78415d",
          "open_late": false,
          "start": "2019-01-18T06:00:42.000-08:00",
          "start_hour": 10,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-05-01T13:03:22.549-07:00",
          "days": [
            3
          ],
          "end": "2019-05-08T14:00:07.000-07:00",
          "end_hour": 17,
          "end_minutes": 0,
          "id": "5cc9fb8a1ca48e0e5b7eea2f",
          "open_late": false,
          "start": "2019-05-08T07:00:07.000-07:00",
          "start_hour": 10,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-05-01T13:03:22.701-07:00",
          "days": [
            4
          ],
          "end": "2019-05-09T13:00:07.000-07:00",
          "end_hour": 16,
          "end_minutes": 0,
          "id": "5cc9fb8a1ca48e0e5b7eea30",
          "open_late": false,
          "start": "2019-05-09T07:00:07.000-07:00",
          "start_hour": 10,
          "start_minutes": 0,
          "type": "location"
        }
      ],
      "sort_order": 13,
      "type": "menubuilder",
      "webtrition_version": 2
    },
    {
      "_type": "DOC::WebtritionLocation",
      "id": "58c699a13191a2a314665019",
      "name": "Viking Grounds",
      "schedules": [
        {
          "created_at": "2019-01-11T06:50:39.901-08:00",
          "days": [
            1,
            2,
            3,
            4
          ],
          "end": "2019-05-07T16:00:19.000-07:00",
          "end_hour": 19,
          "end_minutes": 0,
          "id": "5c38ad3fbddf43090b78299b",
          "open_late": false,
          "start": "2019-01-14T03:00:19.000-08:00",
          "start_hour": 7,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-01-11T06:50:53.874-08:00",
          "days": [
            5
          ],
          "end": "2019-05-03T11:00:41.000-07:00",
          "end_hour": 14,
          "end_minutes": 0,
          "id": "5c38ad4dbddf4309161e01b9",
          "open_late": false,
          "start": "2019-01-18T03:00:41.000-08:00",
          "start_hour": 7,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-05-01T12:51:54.142-07:00",
          "days": [
            3
          ],
          "end": "2019-05-08T14:00:40.000-07:00",
          "end_hour": 17,
          "end_minutes": 0,
          "id": "5cc9f8da4198d40967eca442",
          "open_late": false,
          "start": "2019-05-08T04:00:40.000-07:00",
          "start_hour": 7,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-05-01T12:52:06.853-07:00",
          "days": [
            4
          ],
          "end": "2019-05-09T11:00:54.000-07:00",
          "end_hour": 14,
          "end_minutes": 0,
          "id": "5cc9f8e64198d4097977f4b1",
          "open_late": false,
          "start": "2019-05-09T04:00:54.000-07:00",
          "start_hour": 7,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-05-01T12:52:22.221-07:00",
          "days": [
            5
          ],
          "end": "2019-05-10T10:00:13.000-07:00",
          "end_hour": 13,
          "end_minutes": 0,
          "id": "5cc9f8f64198d40967ecbf47",
          "open_late": false,
          "start": "2019-05-10T04:00:13.000-07:00",
          "start_hour": 7,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-05-14T08:50:33.575-07:00",
          "days": [
            1,
            2,
            3,
            4
          ],
          "end": "2019-08-02T11:00:16.000-07:00",
          "end_hour": 14,
          "end_minutes": 0,
          "id": "5cdae3c91ca48e0c2ff25579",
          "open_late": false,
          "start": "2019-05-20T05:00:16.000-07:00",
          "start_hour": 8,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-05-14T08:50:42.781-07:00",
          "days": [
            5
          ],
          "end": "2019-08-02T10:00:35.000-07:00",
          "end_hour": 13,
          "end_minutes": 0,
          "id": "5cdae3d21ca48e0c2ff2557a",
          "open_late": false,
          "start": "2019-05-20T05:00:35.000-07:00",
          "start_hour": 8,
          "start_minutes": 0,
          "type": "location"
        }
      ],
      "sort_order": 14,
      "type": null,
      "webtrition_version": 2
    },
    {
      "_type": "DOC::WebtritionLocation",
      "id": "587655acee596f59b1adbe6d",
      "name": "Viking Marketplace",
      "schedules": [
        {
          "created_at": "2019-01-22T09:47:34.548-08:00",
          "days": [
            1,
            2,
            3,
            4
          ],
          "end": "2019-05-03T17:00:02.000-07:00",
          "end_hour": 20,
          "end_minutes": 0,
          "id": "5c4757368e45bf0d3ce069c2",
          "open_late": false,
          "start": "2019-01-22T03:00:02.000-08:00",
          "start_hour": 7,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-01-22T09:47:47.569-08:00",
          "days": [
            5
          ],
          "end": "2019-05-03T16:00:37.000-07:00",
          "end_hour": 19,
          "end_minutes": 0,
          "id": "5c4757438e45bf0d7e734e51",
          "open_late": false,
          "start": "2019-01-22T03:00:37.000-08:00",
          "start_hour": 7,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-01-22T12:44:47.386-08:00",
          "days": [
            0
          ],
          "end": "2019-05-05T17:00:37.000-07:00",
          "end_hour": 20,
          "end_minutes": 0,
          "id": "5c4780bf8e45bf0f9714d1fa",
          "open_late": false,
          "start": "2019-01-22T06:00:37.000-08:00",
          "start_hour": 10,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-01-22T12:47:14.481-08:00",
          "days": [
            6
          ],
          "end": "2019-05-04T16:00:03.000-07:00",
          "end_hour": 19,
          "end_minutes": 0,
          "id": "5c4781528e45bf0f781de1fa",
          "open_late": false,
          "start": "2019-02-17T06:00:03.000-08:00",
          "start_hour": 10,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-05-01T12:40:49.198-07:00",
          "days": [
            1,
            2,
            3,
            4
          ],
          "end": "2019-05-09T17:00:34.000-07:00",
          "end_hour": 20,
          "end_minutes": 0,
          "id": "5cc9f6411ca48e0a252753aa",
          "open_late": false,
          "start": "2019-05-06T04:00:34.000-07:00",
          "start_hour": 7,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-05-01T12:41:35.195-07:00",
          "days": [
            5
          ],
          "end": "2019-05-10T13:00:17.000-07:00",
          "end_hour": 16,
          "end_minutes": 0,
          "id": "5cc9f66f1ca48e0a2e094bc0",
          "open_late": false,
          "start": "2019-05-10T04:00:17.000-07:00",
          "start_hour": 7,
          "start_minutes": 0,
          "type": "location"
        },
        {
          "created_at": "2019-05-14T08:49:39.214-07:00",
          "days": [
            1,
            2,
            3,
            4,
            5
          ],
          "end": "2019-08-02T11:00:27.000-07:00",
          "end_hour": 14,
          "end_minutes": 0,
          "id": "5cdae3931ca48e0c240472ba",
          "open_late": false,
          "start": "2019-05-20T08:00:27.000-07:00",
          "start_hour": 11,
          "start_minutes": 0,
          "type": "location"
        }
      ],
      "sort_order": 0,
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

| Parameter | Required | Description                                    |
| --------- | -------- | ---------------------------------------------- |
| site_id   | yes      | The Id of your site should be provided to you. |
| timestamp | yes      | Formatted as YYYY-MM-DD                        |

<aside class="success">
Request volumes are logged and monitored. Please don't be spammy with your services 😀.
</aside>