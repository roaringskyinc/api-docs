---
title: Dine On Campus&reg; API 0.6b

language_tabs: # must be one of https://git.io/vQNgJ
  - shell
  # - ruby
  # - python
  # - javascript

toc_footers:
  # - <a href='#'>Sign Up for a Developer Key</a>
  # - <a href='https://github.com/lord/slate'>Documentation Powered by Slate</a>

includes:
  - locations
  - events
  - specials
  - staff
  - errors

search: true
---

# Introduction

Welcome to the **Dine On Campus**&reg; API! You can use the API to access events, specials, staff, locations, and menus. We'll be adding more in the near future.

You can view code examples in the area to the right.

# Authentication

> To authorize, use this code:

```shell
# With shell, you can just pass the correct header with each request
curl -XPOST -sk -F 'email={email}' -F 'password={password}' https://kapi.dineoncampus.com/token
```

**Dine On Campus**&reg; uses API tokens for access on a per-developer basis. To request access for an additional developer &mdash; for now &mdash; please contact Dylan Bromby (dylan@roaringsky.com). We'll be automating this process in the near future.

**Dine On Campus**&reg; expects the API token to be included in request headers:

`Authorization: Bearer {token}`

<aside class="notice">
You must replace <code>{token}</code> with your personal API token.
</aside>

# Menu

## Get a single menu

```shell
curl -H "Authorization: Bearer {token}" https://kapi.dineoncampus.com/location/menu
```

> The above command returns JSON structured like this:

```json
{
  "allergen_filter": false,
  "menu": {
    "date": "2019-07-08",
    "from_date": null,
    "id": "5d23f9374198d409c3061864",
    "name": null,
    "periods": [
      {
        "categories": [
          {
            "id": "5d23f9384198d409c306186b",
            "items": [
              {
                "calories": 10,
                "custom_allergens": [],
                "desc": "Leaf lettuce, tomato slice, pickle slices",
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd1",
                    "name": "Tomato",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff3",
                    "name": "Mustard*",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5743191a24f12b53028",
                    "name": "Beef*",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5743191a24f12b5302a",
                    "name": "Pork*",
                    "type": "allergen"
                  }
                ],
                "id": "59e4ffcc28d0e73e15f812d7",
                "ingredients": "Tomatoes Fresh Each Slice 1/2\", Pickles Dill Hamburger Slices, Lettuce Leaf Individual Leaf Fresh",
                "mrn": "13163",
                "mrn_full": "13163.0",
                "name": "Burger Accompaniments",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061b60",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "10",
                    "value_numeric": "10"
                  },
                  {
                    "id": "5d23f9594198d409c3061b61",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061b62",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061b63",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061b64",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061b65",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061b66",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "170",
                    "value_numeric": "170"
                  },
                  {
                    "id": "5d23f9594198d409c3061b67",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061b68",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "2",
                    "value_numeric": "2"
                  },
                  {
                    "id": "5d23f9594198d409c3061b69",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061b6a",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061b6b",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "1 serving(s)",
                "qty": null,
                "rev": "0",
                "sort_order": 1,
                "webtrition_id": 115334070
            
            ],
            "name": "Grill",
            "sort_order": 0
          },
          {
            "id": "5d23f9384198d409c306186c",
            "items": [
              {
                "calories": 190,
                "custom_allergens": [],
                "desc": "Chicken breasts marinated in Lemon Dijon vinaigrette and pan seared",
                "filters": [
                  {
                    "id": "5934c5733191a24f12b52fef",
                    "name": "Alcohol",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5743191a24f12b53029",
                    "name": "Mustard",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c576ee596f19f2126a40",
                    "name": "Poultry",
                    "type": "allergen"
                  },
                  {
                    "id": "5a67f531a4227a2fac230c8e",
                    "name": "Balanced U",
                    "type": "label"
                  }
                ],
                "id": "59ee92e528d0e73e15f87965",
                "ingredients": "Chicken Breast Boneless Skinless Random Raw, Oil Olive, Juice Lemon Fresh, Mustard Dijon, Honey, Oregano Fresh Chopped, Salt Kosher, Spice Pepper Black Ground",
                "mrn": "59037",
                "mrn_full": "59037.2",
                "name": "Lemon Oregano Chicken",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061ba8",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "190",
                    "value_numeric": "190"
                  },
                  {
                    "id": "5d23f9594198d409c3061ba9",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "80",
                    "value_numeric": "80"
                  },
                  {
                    "id": "5d23f9594198d409c3061baa",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "70",
                    "value_numeric": "70"
                  },
                  {
                    "id": "5d23f9594198d409c3061bab",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061bac",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "26",
                    "value_numeric": "26"
                  },
                  {
                    "id": "5d23f9594198d409c3061bad",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "1.5",
                    "value_numeric": "1.5"
                  },
                  {
                    "id": "5d23f9594198d409c3061bae",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "125",
                    "value_numeric": "125"
                  },
                  {
                    "id": "5d23f9594198d409c3061baf",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061bb0",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061bb1",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "9",
                    "value_numeric": "9"
                  },
                  {
                    "id": "5d23f9594198d409c3061bb2",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "-",
                    "value_numeric": "-"
                  },
                  {
                    "id": "5d23f9594198d409c3061bb3",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "5+",
                    "value_numeric": "5+"
                  }
                ],
                "portion": "4 oz meat",
                "qty": null,
                "rev": "2",
                "sort_order": 1,
                "webtrition_id": 115334090
              }              
            ],
            "name": "Mongolian",
            "sort_order": 1
          }
        ],
        "id": "5d23f9384198d409c306186a",
        "name": "Lunch",
        "sort_order": 0
      }
    ],
    "to_date": null
  },
  "records": 1,
  "request_time": 0.032709555,
  "status": "success"
}
```

This endpoint retrieves a menu for a specific day.

### HTTP Request

`GET http://kapi.dineoncampus.com/location/menu`

### Query Parameters

| Parameter   | Required | Description                                                     |
| ----------- | -------- | --------------------------------------------------------------- |
| site_id     | yes      | The Id of your site should be provided to you.                  |
| location_id | yes      | The location Id. Obtained using the `/locations/open` endpoint. |
| platform    | yes      | Should be set to 0.                                             |
| date        | yes      | Formatted as YYYY-MM-DD                                         |

<aside class="success">
Request volumes are logged and monitored. Request thresholds will be enforced in the near future 😀.
</aside>
