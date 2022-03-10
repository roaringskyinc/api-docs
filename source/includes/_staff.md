# Staff

## Get staff

```shell
curl -H "Authorization: Bearer {token}" https://kapi.dineoncampus.com/staff
```

> The above command returns JSON structured like this:

```json
{
  "staff": [
    {
      "id": "5ac2df8ff3eeb600c67c22b9",
      "first_name": "First name",
      "last_name": "Last name",
      "title": "Title",
      "bio": "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean quis lectus ut orci aliquam rhoncus. Suspendisse imperdiet ut risus eget posuere. Donec eu dapibus nulla, dapibus pharetra nisi. Ut porttitor velit non aliquet congue. In at felis tincidunt, gravida ligula ac, lobortis enim. Vestibulum eget lorem efficitur, euismod augue in, vulputate purus. Nulla accumsan velit non mollis vulputate.",
      "email": "Email address",
      "active": true,
      "phone": "0000000000",
      "sort_order": 0,
      "phone_formatted": "(000) 000 - 0000",
      "picture": {
        "id": "6196e066a9f13a36eadf7349",
        "file_name": "https://api.dineoncampus.com/files/staff/0e2b7c78-7dd8-4aad-892b-11aa64c1a23f.jpg"
      }
    }
  ]
}
```

This endpoint retrieves all active staff.

### HTTP Request

`GET http://kapi.dineoncampus.com/staff`

### Query Parameters

| Parameter | Required | Description                                    |
| --------- | -------- | ---------------------------------------------- |
| site_id   | yes      | The Id of your site should be provided to you. |

<aside class="success">
Request volumes are logged and monitored. Request thresholds will be enforced in the near future 😀.
</aside>