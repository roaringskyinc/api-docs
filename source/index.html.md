---
title: API Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - shell
  # - ruby
  # - python
  # - javascript

toc_footers:
  - <a href='#'>Sign Up for a Developer Key</a>
  - <a href='https://github.com/lord/slate'>Documentation Powered by Slate</a>

includes:
  - errors

search: true
---

# Introduction

Welcome to the Nutricloud API! You can use the API to access events, special offers, locations, and menus. We'll be adding more in the near future.

You can view code examples in the dark area to the right.

# Authentication

> To authorize, use this code:

```shell
# With shell, you can just pass the correct header with each request
curl -XPOST -sk -F 'email={email}' -F 'password={password}' https://kapi.dineoncampus.com/{key}
```

> Make sure to replace `{key}` with your API key.

Nutricloud uses API tokens for access on a per-developer basis. To request a new developer account please contact Dylan Bromby (dylan@roaringsky.com).

Nutricloud expects the API token to be included in request headers:

`Authorization: {token}`

<aside class="notice">
You must replace <code>{token}</code> with your personal API token.
</aside>

# Menu

## Get a single menu

```shell
curl -H "Authorization: Bearer {token}" https://kapi.dineoncampus.com/location/menu
  -H "Authorization: {token}"
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
              },
              {
                "calories": 310,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fcf",
                    "name": "Onion",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd1",
                    "name": "Tomato",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5733191a24f12b52fdf",
                    "name": "Gluten",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe0",
                    "name": "Milk",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe2",
                    "name": "Wheat",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff1",
                    "name": "Egg",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff2",
                    "name": "Garlic",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b53002",
                    "name": "Soy",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5753191a24f12b5305b",
                    "name": "MSG*",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c580ee596f19fb1104bf",
                    "name": "Alcohol*",
                    "type": "allergen"
                  }
                ],
                "id": "5cfcbc66e67a2d1b3b3faeac",
                "ingredients": "Black Bean Burger Meatless 3.3 oz, Bun Hamburger Wheat 4\", Tomatoes Fresh Each Slice, Lettuce Leaf Individual Leaf Fresh, Oil Cooking Spray",
                "mrn": "75735",
                "mrn_full": "75735.0",
                "name": "Blackbean burger ",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061b6c",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "310",
                    "value_numeric": "310"
                  },
                  {
                    "id": "5d23f9594198d409c3061b6d",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "60",
                    "value_numeric": "60"
                  },
                  {
                    "id": "5d23f9594198d409c3061b6e",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061b6f",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "7",
                    "value_numeric": "7"
                  },
                  {
                    "id": "5d23f9594198d409c3061b70",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "20",
                    "value_numeric": "20"
                  },
                  {
                    "id": "5d23f9594198d409c3061b71",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "1",
                    "value_numeric": "1"
                  },
                  {
                    "id": "5d23f9594198d409c3061b72",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "720",
                    "value_numeric": "720"
                  },
                  {
                    "id": "5d23f9594198d409c3061b73",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "6",
                    "value_numeric": "6"
                  },
                  {
                    "id": "5d23f9594198d409c3061b74",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "43",
                    "value_numeric": "43"
                  },
                  {
                    "id": "5d23f9594198d409c3061b75",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "7",
                    "value_numeric": "7"
                  },
                  {
                    "id": "5d23f9594198d409c3061b76",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061b77",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0+",
                    "value_numeric": "0+"
                  }
                ],
                "portion": "1 serving(s)",
                "qty": null,
                "rev": "0",
                "sort_order": 1,
                "webtrition_id": 115334069
              },
              {
                "calories": 300,
                "custom_allergens": [],
                "desc": "Ground sirloin patty grilled to perfection and served on a bun with lettuce and tomatoes.",
                "filters": [
                  {
                    "id": "5934c5733191a24f12b52fdf",
                    "name": "Gluten",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe2",
                    "name": "Wheat",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b53002",
                    "name": "Soy",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5763191a24f12b530b1",
                    "name": "Beef",
                    "type": "allergen"
                  },
                  {
                    "id": "5a67f531a4227a2fac230c8e",
                    "name": "Balanced U",
                    "type": "label"
                  }
                ],
                "id": "59e3eb6428d0e73e15f7a532",
                "ingredients": "Beef Patty 20% Fat Raw 3.2 oz Frozen, Bun Hamburger Wheat 4\"",
                "mrn": "5305",
                "mrn_full": "5305.14",
                "name": "Hamburger on Bun",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061b78",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "300",
                    "value_numeric": "300"
                  },
                  {
                    "id": "5d23f9594198d409c3061b79",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "120",
                    "value_numeric": "120"
                  },
                  {
                    "id": "5d23f9594198d409c3061b7a",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "55",
                    "value_numeric": "55"
                  },
                  {
                    "id": "5d23f9594198d409c3061b7b",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061b7c",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "21",
                    "value_numeric": "21"
                  },
                  {
                    "id": "5d23f9594198d409c3061b7d",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "4.5",
                    "value_numeric": "4.5"
                  },
                  {
                    "id": "5d23f9594198d409c3061b7e",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "290",
                    "value_numeric": "290"
                  },
                  {
                    "id": "5d23f9594198d409c3061b7f",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "4",
                    "value_numeric": "4"
                  },
                  {
                    "id": "5d23f9594198d409c3061b80",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "24",
                    "value_numeric": "24"
                  },
                  {
                    "id": "5d23f9594198d409c3061b81",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "13",
                    "value_numeric": "13"
                  },
                  {
                    "id": "5d23f9594198d409c3061b82",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061b83",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "1 sandwich",
                "qty": null,
                "rev": "14",
                "sort_order": 2,
                "webtrition_id": 115334072
              },
              {
                "calories": 430,
                "custom_allergens": [],
                "desc": "Seasoned ground turkey",
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fcf",
                    "name": "Onion",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fdf",
                    "name": "Gluten",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe2",
                    "name": "Wheat",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff2",
                    "name": "Garlic",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b53002",
                    "name": "Soy",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c576ee596f19f2126a40",
                    "name": "Poultry",
                    "type": "allergen"
                  }
                ],
                "id": "5d0786d2e67a2d1b3bab4f8a",
                "ingredients": "Turkey Burger Savory 4 oz Raw, Bun Hamburger Whole Wheat 4\" 2.25 oz, Lettuce Leaf Individual Leaf Fresh, Oil Canola",
                "mrn": "5816",
                "mrn_full": "5816.6",
                "name": "Turkey Burger",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061b84",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "430",
                    "value_numeric": "430"
                  },
                  {
                    "id": "5d23f9594198d409c3061b85",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "190",
                    "value_numeric": "190"
                  },
                  {
                    "id": "5d23f9594198d409c3061b86",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "95",
                    "value_numeric": "95"
                  },
                  {
                    "id": "5d23f9594198d409c3061b87",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "5",
                    "value_numeric": "5"
                  },
                  {
                    "id": "5d23f9594198d409c3061b88",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "26",
                    "value_numeric": "26"
                  },
                  {
                    "id": "5d23f9594198d409c3061b89",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "5",
                    "value_numeric": "5"
                  },
                  {
                    "id": "5d23f9594198d409c3061b8a",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "680",
                    "value_numeric": "680"
                  },
                  {
                    "id": "5d23f9594198d409c3061b8b",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "6",
                    "value_numeric": "6"
                  },
                  {
                    "id": "5d23f9594198d409c3061b8c",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "36",
                    "value_numeric": "36"
                  },
                  {
                    "id": "5d23f9594198d409c3061b8d",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "21",
                    "value_numeric": "21"
                  },
                  {
                    "id": "5d23f9594198d409c3061b8e",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "-",
                    "value_numeric": "-"
                  },
                  {
                    "id": "5d23f9594198d409c3061b8f",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "10",
                    "value_numeric": "10"
                  }
                ],
                "portion": "1 each",
                "qty": null,
                "rev": "6",
                "sort_order": 2,
                "webtrition_id": 115334071
              },
              {
                "calories": 190,
                "custom_allergens": [],
                "desc": "french fries",
                "filters": [
                  {
                    "id": "5934c5733191a24f12b53002",
                    "name": "Soy",
                    "type": "allergen"
                  }
                ],
                "id": "59e3e93828d0e73e15f7a1a6",
                "ingredients": "Potatoes French Fries 3/8\" Frozen",
                "mrn": "8414",
                "mrn_full": "8414.0",
                "name": "French Fries",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061b90",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "190",
                    "value_numeric": "190"
                  },
                  {
                    "id": "5d23f9594198d409c3061b91",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "90",
                    "value_numeric": "90"
                  },
                  {
                    "id": "5d23f9594198d409c3061b92",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061b93",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "2",
                    "value_numeric": "2"
                  },
                  {
                    "id": "5d23f9594198d409c3061b94",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "2",
                    "value_numeric": "2"
                  },
                  {
                    "id": "5d23f9594198d409c3061b95",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "1",
                    "value_numeric": "1"
                  },
                  {
                    "id": "5d23f9594198d409c3061b96",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "20",
                    "value_numeric": "20"
                  },
                  {
                    "id": "5d23f9594198d409c3061b97",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061b98",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "21",
                    "value_numeric": "21"
                  },
                  {
                    "id": "5d23f9594198d409c3061b99",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "10",
                    "value_numeric": "10"
                  },
                  {
                    "id": "5d23f9594198d409c3061b9a",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "-",
                    "value_numeric": "-"
                  },
                  {
                    "id": "5d23f9594198d409c3061b9b",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "3 ounce",
                "qty": null,
                "rev": "0",
                "sort_order": 3,
                "webtrition_id": 115334073
              },
              {
                "calories": 230,
                "custom_allergens": [],
                "desc": "Tender beef in a rich sauce with beans and tomatoes",
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fcf",
                    "name": "Onion",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd1",
                    "name": "Tomato",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff2",
                    "name": "Garlic",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff3",
                    "name": "Mustard*",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b53002",
                    "name": "Soy",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5753191a24f12b5305b",
                    "name": "MSG*",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5763191a24f12b530b1",
                    "name": "Beef",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c57bee596f19f2126c69",
                    "name": "Celery*",
                    "type": "allergen"
                  },
                  {
                    "id": "5a67f531a4227a2fac230c8e",
                    "name": "Balanced U",
                    "type": "label"
                  }
                ],
                "id": "59ee066d28d0e73e15f871eb",
                "ingredients": "Beef Ground 80/20 Raw, Water Hot, Beans Kidney Dark Red Canned Including Liquids, Tomato Puree Canned, Onions Yellow Fresh Chopped Fine, Peppers Bell Green Fresh Chopped, Spice Chili Powder Light, Sugar Granulated, Base Beef Maggi, Salt Bulk, Spice Cumin Ground, Spice Pepper Black Ground, Spice Pepper Cayenne",
                "mrn": "4843",
                "mrn_full": "4843.0",
                "name": "Beef Chili",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061b9c",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "230",
                    "value_numeric": "230"
                  },
                  {
                    "id": "5d23f9594198d409c3061b9d",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "100",
                    "value_numeric": "100"
                  },
                  {
                    "id": "5d23f9594198d409c3061b9e",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "55",
                    "value_numeric": "55"
                  },
                  {
                    "id": "5d23f9594198d409c3061b9f",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "4",
                    "value_numeric": "4"
                  },
                  {
                    "id": "5d23f9594198d409c3061ba0",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "20",
                    "value_numeric": "20"
                  },
                  {
                    "id": "5d23f9594198d409c3061ba1",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "4",
                    "value_numeric": "4"
                  },
                  {
                    "id": "5d23f9594198d409c3061ba2",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "320",
                    "value_numeric": "320"
                  },
                  {
                    "id": "5d23f9594198d409c3061ba3",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "3",
                    "value_numeric": "3"
                  },
                  {
                    "id": "5d23f9594198d409c3061ba4",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "13",
                    "value_numeric": "13"
                  },
                  {
                    "id": "5d23f9594198d409c3061ba5",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "11",
                    "value_numeric": "11"
                  },
                  {
                    "id": "5d23f9594198d409c3061ba6",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "-",
                    "value_numeric": "-"
                  },
                  {
                    "id": "5d23f9594198d409c3061ba7",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0+",
                    "value_numeric": "0+"
                  }
                ],
                "portion": "8 oz portion",
                "qty": null,
                "rev": "0",
                "sort_order": 4,
                "webtrition_id": 115334074
              }
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
              },
              {
                "calories": 160,
                "custom_allergens": [],
                "desc": "Long grain rice simply steamed",
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  },
                  {
                    "id": "5a67f531a4227a2fac230c8e",
                    "name": "Balanced U",
                    "type": "label"
                  }
                ],
                "id": "5a60107a28d0e73e15f91ced",
                "ingredients": "Water, Rice White Long Grain Converted Dry",
                "mrn": "28232",
                "mrn_full": "28232.0",
                "name": "Steamed Rice",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061bb4",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "160",
                    "value_numeric": "160"
                  },
                  {
                    "id": "5d23f9594198d409c3061bb5",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061bb6",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061bb7",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061bb8",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "3",
                    "value_numeric": "3"
                  },
                  {
                    "id": "5d23f9594198d409c3061bb9",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061bba",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061bbb",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061bbc",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "34",
                    "value_numeric": "34"
                  },
                  {
                    "id": "5d23f9594198d409c3061bbd",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061bbe",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "-",
                    "value_numeric": "-"
                  },
                  {
                    "id": "5d23f9594198d409c3061bbf",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "3/4 cup",
                "qty": null,
                "rev": "0",
                "sort_order": 2,
                "webtrition_id": 115334091
              },
              {
                "calories": 45,
                "custom_allergens": [],
                "desc": "Freshly steamed seasoned broccoli",
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  },
                  {
                    "id": "596e6e8aee596fc1869461d3",
                    "name": "Avoiding Gluten",
                    "type": "label"
                  }
                ],
                "id": "59e3d8c928d0e73e15f78cd0",
                "ingredients": "Broccoli Fresh Florets, Salt Bulk, Spice Pepper Black Ground",
                "mrn": "103333",
                "mrn_full": "103333.0",
                "name": "Steamed Broccoli",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061bc0",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "45",
                    "value_numeric": "45"
                  },
                  {
                    "id": "5d23f9594198d409c3061bc1",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061bc2",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061bc3",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "4",
                    "value_numeric": "4"
                  },
                  {
                    "id": "5d23f9594198d409c3061bc4",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "4",
                    "value_numeric": "4"
                  },
                  {
                    "id": "5d23f9594198d409c3061bc5",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061bc6",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "280",
                    "value_numeric": "280"
                  },
                  {
                    "id": "5d23f9594198d409c3061bc7",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "2",
                    "value_numeric": "2"
                  },
                  {
                    "id": "5d23f9594198d409c3061bc8",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "9",
                    "value_numeric": "9"
                  },
                  {
                    "id": "5d23f9594198d409c3061bc9",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0.5",
                    "value_numeric": "0.5"
                  },
                  {
                    "id": "5d23f9594198d409c3061bca",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061bcb",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "1 cup",
                "qty": null,
                "rev": "0",
                "sort_order": 3,
                "webtrition_id": 115334092
              }
            ],
            "name": "Mongolian",
            "sort_order": 1
          },
          {
            "id": "5d23f9384198d409c306186d",
            "items": [
              {
                "calories": 830,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd1",
                    "name": "Tomato",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe0",
                    "name": "Milk",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff2",
                    "name": "Garlic",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b53002",
                    "name": "Soy",
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
                  },
                  {
                    "id": "5934c742ee596f19fb110726",
                    "name": "Egg*",
                    "type": "allergen"
                  },
                  {
                    "id": "596e6e8aee596fc1869461d3",
                    "name": "Avoiding Gluten",
                    "type": "label"
                  }
                ],
                "id": "5cfc5740e67a2d1b3b27f7c6",
                "ingredients": "Pizza Crust Richs Gluten Free Par-baked 10\" 7.75 oz Frozen, Cheese Mozzarella Part Skim Pre-Shredded, Tomatoes Crushed Canned Including Liquids, Cheese Parmesan Grated, Spice Garlic Powder, Spice Oregano Dried Crumbled, Spice Pepper Red Chili Crushed Flakes",
                "mrn": "68052",
                "mrn_full": "68052.0",
                "name": "Cheese Pizza",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061bcc",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "830",
                    "value_numeric": "830"
                  },
                  {
                    "id": "5d23f9594198d409c3061bcd",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "240",
                    "value_numeric": "240"
                  },
                  {
                    "id": "5d23f9594198d409c3061bce",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "40",
                    "value_numeric": "40"
                  },
                  {
                    "id": "5d23f9594198d409c3061bcf",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "4",
                    "value_numeric": "4"
                  },
                  {
                    "id": "5d23f9594198d409c3061bd0",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "23",
                    "value_numeric": "23"
                  },
                  {
                    "id": "5d23f9594198d409c3061bd1",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "12",
                    "value_numeric": "12"
                  },
                  {
                    "id": "5d23f9594198d409c3061bd2",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "1400",
                    "value_numeric": "1400"
                  },
                  {
                    "id": "5d23f9594198d409c3061bd3",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "10+",
                    "value_numeric": "10+"
                  },
                  {
                    "id": "5d23f9594198d409c3061bd4",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "125",
                    "value_numeric": "125"
                  },
                  {
                    "id": "5d23f9594198d409c3061bd5",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "27",
                    "value_numeric": "27"
                  },
                  {
                    "id": "5d23f9594198d409c3061bd6",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0.5+",
                    "value_numeric": "0.5+"
                  },
                  {
                    "id": "5d23f9594198d409c3061bd7",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "10+",
                    "value_numeric": "10+"
                  }
                ],
                "portion": "1 each",
                "qty": null,
                "rev": "0",
                "sort_order": 1,
                "webtrition_id": 115334094
              },
              {
                "calories": 500,
                "custom_allergens": [],
                "desc": "Zesty Meatball Pizza",
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fcf",
                    "name": "Onion",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd1",
                    "name": "Tomato",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fdf",
                    "name": "Gluten",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe0",
                    "name": "Milk",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe2",
                    "name": "Wheat",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff2",
                    "name": "Garlic",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff3",
                    "name": "Mustard*",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b53002",
                    "name": "Soy",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5753191a24f12b5305b",
                    "name": "MSG*",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5763191a24f12b530b1",
                    "name": "Beef",
                    "type": "allergen"
                  }
                ],
                "id": "5d0786d2e67a2d1b3bab4fac",
                "ingredients": "Dough Pizza 16” FTO Whole Grain Rolled Edge Frozen, Cheese Mozzarella Part Skim Pre-Shredded, Meatballs Beef Cooked .5 oz Frozen, Sauce Pizza Canned, Cornmeal Plain Yellow, Oil Canola, Cheese Parmesan Grated, Parsley Fresh Minced, Garlic Cloves Peeled Fresh Chopped, Parsley Fresh Chopped, Spice Garlic Powder, Seasoning Italian, Spice Oregano Dried Crumbled, Spice Pepper Red Chili Crushed Flakes",
                "mrn": "32767",
                "mrn_full": "32767.3",
                "name": "Meatball Pizza ",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061bd8",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "500",
                    "value_numeric": "500"
                  },
                  {
                    "id": "5d23f9594198d409c3061bd9",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "190",
                    "value_numeric": "190"
                  },
                  {
                    "id": "5d23f9594198d409c3061bda",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "55+",
                    "value_numeric": "55+"
                  },
                  {
                    "id": "5d23f9594198d409c3061bdb",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "6",
                    "value_numeric": "6"
                  },
                  {
                    "id": "5d23f9594198d409c3061bdc",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "27",
                    "value_numeric": "27"
                  },
                  {
                    "id": "5d23f9594198d409c3061bdd",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "9",
                    "value_numeric": "9"
                  },
                  {
                    "id": "5d23f9594198d409c3061bde",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "960",
                    "value_numeric": "960"
                  },
                  {
                    "id": "5d23f9594198d409c3061bdf",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "6+",
                    "value_numeric": "6+"
                  },
                  {
                    "id": "5d23f9594198d409c3061be0",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "50",
                    "value_numeric": "50"
                  },
                  {
                    "id": "5d23f9594198d409c3061be1",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "21",
                    "value_numeric": "21"
                  },
                  {
                    "id": "5d23f9594198d409c3061be2",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "-",
                    "value_numeric": "-"
                  },
                  {
                    "id": "5d23f9594198d409c3061be3",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "5+",
                    "value_numeric": "5+"
                  }
                ],
                "portion": "1 slice",
                "qty": null,
                "rev": "3",
                "sort_order": 1,
                "webtrition_id": 115334093
              },
              {
                "calories": 420,
                "custom_allergens": [],
                "desc": "Rich sausage and roasted mushrooms topped with mozzarella cheese",
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fcf",
                    "name": "Onion",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd1",
                    "name": "Tomato",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fdf",
                    "name": "Gluten",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe0",
                    "name": "Milk",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe2",
                    "name": "Wheat",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fef",
                    "name": "Alcohol",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff2",
                    "name": "Garlic",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff4",
                    "name": "Pork",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b53002",
                    "name": "Soy",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5743191a24f12b53029",
                    "name": "Mustard",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5773191a24f12b53121",
                    "name": "Mushroom",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c57bee596f19f2126c69",
                    "name": "Celery*",
                    "type": "allergen"
                  }
                ],
                "id": "5d016a6be67a2d1b3bec00ba",
                "ingredients": "Dough Pizza 16” FTO Whole Grain Rolled Edge Frozen, Cheese Mozzarella Part Skim Pre-Shredded, Mushrooms Portobello Fresh, Sauce Pizza Canned, Sausage Pork Crumbles Italian FC, Salad Dressing Balsamic Bulk, Cornmeal Plain Yellow, Oil Canola, Cheese Parmesan Grated, Thyme Fresh Minced, Garlic Cloves Peeled Fresh Chopped, Parsley Fresh Chopped, Spice Garlic Powder, Seasoning Italian, Spice Oregano Dried Crumbled, Spice Pepper Red Chili Crushed Flakes",
                "mrn": "32835",
                "mrn_full": "32835.0",
                "name": "Sausage and Mushroom Pizza",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061be4",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "420",
                    "value_numeric": "420"
                  },
                  {
                    "id": "5d23f9594198d409c3061be5",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "140",
                    "value_numeric": "140"
                  },
                  {
                    "id": "5d23f9594198d409c3061be6",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "35+",
                    "value_numeric": "35+"
                  },
                  {
                    "id": "5d23f9594198d409c3061be7",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "6",
                    "value_numeric": "6"
                  },
                  {
                    "id": "5d23f9594198d409c3061be8",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "21",
                    "value_numeric": "21"
                  },
                  {
                    "id": "5d23f9594198d409c3061be9",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "6",
                    "value_numeric": "6"
                  },
                  {
                    "id": "5d23f9594198d409c3061bea",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "870",
                    "value_numeric": "870"
                  },
                  {
                    "id": "5d23f9594198d409c3061beb",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "7+",
                    "value_numeric": "7+"
                  },
                  {
                    "id": "5d23f9594198d409c3061bec",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "49",
                    "value_numeric": "49"
                  },
                  {
                    "id": "5d23f9594198d409c3061bed",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "16",
                    "value_numeric": "16"
                  },
                  {
                    "id": "5d23f9594198d409c3061bee",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "-",
                    "value_numeric": "-"
                  },
                  {
                    "id": "5d23f9594198d409c3061bef",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "10+",
                    "value_numeric": "10+"
                  }
                ],
                "portion": "1 slice",
                "qty": null,
                "rev": "0",
                "sort_order": 2,
                "webtrition_id": 115334095
              },
              {
                "calories": 500,
                "custom_allergens": [],
                "desc": "Tangy sauce, melted mozzarella and crisp pepperoni",
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fcf",
                    "name": "Onion",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd1",
                    "name": "Tomato",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fdf",
                    "name": "Gluten",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe0",
                    "name": "Milk",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe2",
                    "name": "Wheat",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff2",
                    "name": "Garlic",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff3",
                    "name": "Mustard*",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff4",
                    "name": "Pork",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b53002",
                    "name": "Soy",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5763191a24f12b530b1",
                    "name": "Beef",
                    "type": "allergen"
                  }
                ],
                "id": "59e3d70628d0e73e15f78afd",
                "ingredients": "Dough Pizza 16\" Pre-sheeted Rolled Edge 29.5 oz Frozen, Sauce Pizza Canned, Pepperoni Pre-Sliced, Cheese Mozzarella Whole Milk Pre-Shredded, Cheese Parmesan Grated, Oil Canola",
                "mrn": "2154",
                "mrn_full": "2154.0",
                "name": "Pepperoni Pizza",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061bf0",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "500",
                    "value_numeric": "500"
                  },
                  {
                    "id": "5d23f9594198d409c3061bf1",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "200",
                    "value_numeric": "200"
                  },
                  {
                    "id": "5d23f9594198d409c3061bf2",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "45+",
                    "value_numeric": "45+"
                  },
                  {
                    "id": "5d23f9594198d409c3061bf3",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "4",
                    "value_numeric": "4"
                  },
                  {
                    "id": "5d23f9594198d409c3061bf4",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "21",
                    "value_numeric": "21"
                  },
                  {
                    "id": "5d23f9594198d409c3061bf5",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "10",
                    "value_numeric": "10"
                  },
                  {
                    "id": "5d23f9594198d409c3061bf6",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "1230",
                    "value_numeric": "1230"
                  },
                  {
                    "id": "5d23f9594198d409c3061bf7",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "4",
                    "value_numeric": "4"
                  },
                  {
                    "id": "5d23f9594198d409c3061bf8",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "52",
                    "value_numeric": "52"
                  },
                  {
                    "id": "5d23f9594198d409c3061bf9",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "22",
                    "value_numeric": "22"
                  },
                  {
                    "id": "5d23f9594198d409c3061bfa",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "-",
                    "value_numeric": "-"
                  },
                  {
                    "id": "5d23f9594198d409c3061bfb",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "15+",
                    "value_numeric": "15+"
                  }
                ],
                "portion": "1 slice",
                "qty": null,
                "rev": "0",
                "sort_order": 3,
                "webtrition_id": 115334096
              }
            ],
            "name": "Hearthstone Oven",
            "sort_order": 2
          },
          {
            "id": "5d23f9384198d409c306186e",
            "items": [
              {
                "calories": 5,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  },
                  {
                    "id": "5a67f531a4227a2fac230c8e",
                    "name": "Balanced U",
                    "type": "label"
                  }
                ],
                "id": "5c589b98dc5b76af72fa8ae4",
                "ingredients": "Lettuce Romaine Fresh Chopped 1\"",
                "mrn": "47799",
                "mrn_full": "47799.3",
                "name": "Romaine Lettuce",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061bfc",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "5",
                    "value_numeric": "5"
                  },
                  {
                    "id": "5d23f9594198d409c3061bfd",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061bfe",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061bff",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061c00",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c01",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c02",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c03",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c04",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "1",
                    "value_numeric": "1"
                  },
                  {
                    "id": "5d23f9594198d409c3061c05",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c06",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c07",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "3/4 cup",
                "qty": null,
                "rev": "3",
                "sort_order": 1,
                "webtrition_id": 106456768
              },
              {
                "calories": 0,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  },
                  {
                    "id": "5a67f531a4227a2fac230c8e",
                    "name": "Balanced U",
                    "type": "label"
                  }
                ],
                "id": "5c0381bfdc5b76af72fa3d05",
                "ingredients": "Lettuce Arugula Baby Fresh",
                "mrn": "62323",
                "mrn_full": "62323.0",
                "name": "Baby Arugula",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061c08",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c09",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c0a",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c0b",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c0c",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c0d",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c0e",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c0f",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c10",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061c11",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c12",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c13",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "3/4 cup",
                "qty": null,
                "rev": "0",
                "sort_order": 2,
                "webtrition_id": 106456771
              },
              {
                "calories": 150,
                "custom_allergens": [],
                "desc": "Tender and moist",
                "filters": [
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
                "id": "59e4011628d0e73e15f7c7be",
                "ingredients": "Chicken Breast Boneless Skinless Random Raw, Oil Canola, Spice Paprika Ground",
                "mrn": "3904",
                "mrn_full": "3904.0",
                "name": "Grilled Chicken",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061c14",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "150",
                    "value_numeric": "150"
                  },
                  {
                    "id": "5d23f9594198d409c3061c15",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "70",
                    "value_numeric": "70"
                  },
                  {
                    "id": "5d23f9594198d409c3061c16",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "55",
                    "value_numeric": "55"
                  },
                  {
                    "id": "5d23f9594198d409c3061c17",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c18",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "19",
                    "value_numeric": "19"
                  },
                  {
                    "id": "5d23f9594198d409c3061c19",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "1",
                    "value_numeric": "1"
                  },
                  {
                    "id": "5d23f9594198d409c3061c1a",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "45",
                    "value_numeric": "45"
                  },
                  {
                    "id": "5d23f9594198d409c3061c1b",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c1c",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c1d",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "8",
                    "value_numeric": "8"
                  },
                  {
                    "id": "5d23f9594198d409c3061c1e",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "-",
                    "value_numeric": "-"
                  },
                  {
                    "id": "5d23f9594198d409c3061c1f",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "5",
                    "value_numeric": "5"
                  }
                ],
                "portion": "2 oz meat",
                "qty": null,
                "rev": "0",
                "sort_order": 3,
                "webtrition_id": 106456774
              },
              {
                "calories": 60,
                "custom_allergens": [],
                "desc": "Fresh ginger and sesame seeds flavor this grilled tofu",
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff2",
                    "name": "Garlic",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b53002",
                    "name": "Soy",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5763191a24f12b53098",
                    "name": "Orange",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c580ee596f19fb110473",
                    "name": "Sesame Seeds",
                    "type": "allergen"
                  },
                  {
                    "id": "5a67f531a4227a2fac230c8e",
                    "name": "Balanced U",
                    "type": "label"
                  }
                ],
                "id": "5a0afa9d28d0e73e15f8cd88",
                "ingredients": "Tofu Regular Each Slice 4 oz, Ginger Root Fresh Minced, Juice Orange 100%, Spice Sesame Seeds Toasted, Garlic Cloves Peeled Fresh Crushed, Salt Kosher, Spice Pepper Black Ground",
                "mrn": "16090",
                "mrn_full": "16090.2",
                "name": "Grilled Tofu",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061c20",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "60",
                    "value_numeric": "60"
                  },
                  {
                    "id": "5d23f9594198d409c3061c21",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "35",
                    "value_numeric": "35"
                  },
                  {
                    "id": "5d23f9594198d409c3061c22",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c23",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061c24",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "5",
                    "value_numeric": "5"
                  },
                  {
                    "id": "5d23f9594198d409c3061c25",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0.5",
                    "value_numeric": "0.5"
                  },
                  {
                    "id": "5d23f9594198d409c3061c26",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "25",
                    "value_numeric": "25"
                  },
                  {
                    "id": "5d23f9594198d409c3061c27",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061c28",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "2",
                    "value_numeric": "2"
                  },
                  {
                    "id": "5d23f9594198d409c3061c29",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "3.5",
                    "value_numeric": "3.5"
                  },
                  {
                    "id": "5d23f9594198d409c3061c2a",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "-",
                    "value_numeric": "-"
                  },
                  {
                    "id": "5d23f9594198d409c3061c2b",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "2 ounce",
                "qty": null,
                "rev": "2",
                "sort_order": 4,
                "webtrition_id": 106456753
              },
              {
                "calories": 40,
                "custom_allergens": [],
                "desc": "Creamy and delicious.",
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe0",
                    "name": "Milk",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5753191a24f12b5305b",
                    "name": "MSG*",
                    "type": "allergen"
                  },
                  {
                    "id": "5a67f531a4227a2fac230c8e",
                    "name": "Balanced U",
                    "type": "label"
                  }
                ],
                "id": "5a26b2a428d0e73e15f8e6aa",
                "ingredients": "Cottage Cheese Lowfat 1%, Lettuce Leaf Individual Leaf Fresh",
                "mrn": "1746",
                "mrn_full": "1746.4",
                "name": "Cottage Cheese",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061c2c",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "40",
                    "value_numeric": "40"
                  },
                  {
                    "id": "5d23f9594198d409c3061c2d",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "5",
                    "value_numeric": "5"
                  },
                  {
                    "id": "5d23f9594198d409c3061c2e",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "< 5",
                    "value_numeric": "<5"
                  },
                  {
                    "id": "5d23f9594198d409c3061c2f",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c30",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "7",
                    "value_numeric": "7"
                  },
                  {
                    "id": "5d23f9594198d409c3061c31",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c32",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "230",
                    "value_numeric": "230"
                  },
                  {
                    "id": "5d23f9594198d409c3061c33",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "2",
                    "value_numeric": "2"
                  },
                  {
                    "id": "5d23f9594198d409c3061c34",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "2",
                    "value_numeric": "2"
                  },
                  {
                    "id": "5d23f9594198d409c3061c35",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0.5",
                    "value_numeric": "0.5"
                  },
                  {
                    "id": "5d23f9594198d409c3061c36",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "-",
                    "value_numeric": "-"
                  },
                  {
                    "id": "5d23f9594198d409c3061c37",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "2 ounce",
                "qty": null,
                "rev": "4",
                "sort_order": 5,
                "webtrition_id": 106456741
              },
              {
                "calories": 20,
                "custom_allergens": [],
                "desc": "Tangy and delicious.",
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  },
                  {
                    "id": "5934c5763191a24f12b53098",
                    "name": "Orange",
                    "type": "allergen"
                  },
                  {
                    "id": "5a67f531a4227a2fac230c8e",
                    "name": "Balanced U",
                    "type": "label"
                  }
                ],
                "id": "59ee15a328d0e73e15f87405",
                "ingredients": "Orange Mandarin Sections Juice Pack Canned Including Liquids",
                "mrn": "1199",
                "mrn_full": "1199.0",
                "name": "Mandarin Orange Sections",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061c38",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "20",
                    "value_numeric": "20"
                  },
                  {
                    "id": "5d23f9594198d409c3061c39",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c3a",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c3b",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c3c",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c3d",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c3e",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c3f",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "5",
                    "value_numeric": "5"
                  },
                  {
                    "id": "5d23f9594198d409c3061c40",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "5",
                    "value_numeric": "5"
                  },
                  {
                    "id": "5d23f9594198d409c3061c41",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c42",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c43",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "-",
                    "value_numeric": "-"
                  }
                ],
                "portion": "1 ounce",
                "qty": null,
                "rev": "0",
                "sort_order": 6,
                "webtrition_id": 106456759
              },
              {
                "calories": 0,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  },
                  {
                    "id": "5a67f531a4227a2fac230c8e",
                    "name": "Balanced U",
                    "type": "label"
                  }
                ],
                "id": "5c58a6acdc5b76af72fa8ba1",
                "ingredients": "Cucumbers Fresh Scored Sliced Thin Each Slice",
                "mrn": "68562",
                "mrn_full": "68562.0",
                "name": "Sliced Cucumber",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061c44",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c45",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c46",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c47",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c48",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c49",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c4a",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c4b",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c4c",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "1",
                    "value_numeric": "1"
                  },
                  {
                    "id": "5d23f9594198d409c3061c4d",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c4e",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c4f",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "1 ounce",
                "qty": null,
                "rev": "0",
                "sort_order": 7,
                "webtrition_id": 106456762
              },
              {
                "calories": 5,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  },
                  {
                    "id": "5a67f531a4227a2fac230c8e",
                    "name": "Balanced U",
                    "type": "label"
                  }
                ],
                "id": "5af5072217584bbc736d515f",
                "ingredients": "Cauliflower Fresh Florets",
                "mrn": "62528",
                "mrn_full": "62528.0",
                "name": "Cauliflower Florets",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061c50",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "5",
                    "value_numeric": "5"
                  },
                  {
                    "id": "5d23f9594198d409c3061c51",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c52",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c53",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061c54",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061c55",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c56",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "10",
                    "value_numeric": "10"
                  },
                  {
                    "id": "5d23f9594198d409c3061c57",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061c58",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "1",
                    "value_numeric": "1"
                  },
                  {
                    "id": "5d23f9594198d409c3061c59",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c5a",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c5b",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "1 ounce",
                "qty": null,
                "rev": "0",
                "sort_order": 8,
                "webtrition_id": 106456744
              },
              {
                "calories": 15,
                "custom_allergens": [],
                "desc": "Tender Broccoli, lightly seasoned",
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5733191a24f12b53002",
                    "name": "Soy",
                    "type": "allergen"
                  },
                  {
                    "id": "5a67f531a4227a2fac230c8e",
                    "name": "Balanced U",
                    "type": "label"
                  }
                ],
                "id": "59e4e2ca28d0e73e15f80c70",
                "ingredients": "Broccoli Cut Frozen, Margarine Liquid ZTF, Lemon Fresh Wedge",
                "mrn": "1801",
                "mrn_full": "1801.0",
                "name": "Broccoli Cuts",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061c5c",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "15",
                    "value_numeric": "15"
                  },
                  {
                    "id": "5d23f9594198d409c3061c5d",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "5",
                    "value_numeric": "5"
                  },
                  {
                    "id": "5d23f9594198d409c3061c5e",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c5f",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061c60",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061c61",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c62",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "10",
                    "value_numeric": "10"
                  },
                  {
                    "id": "5d23f9594198d409c3061c63",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c64",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "2",
                    "value_numeric": "2"
                  },
                  {
                    "id": "5d23f9594198d409c3061c65",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0.5",
                    "value_numeric": "0.5"
                  },
                  {
                    "id": "5d23f9594198d409c3061c66",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c67",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "1 ounce",
                "qty": null,
                "rev": "0",
                "sort_order": 9,
                "webtrition_id": 106456756
              },
              {
                "calories": 5,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd1",
                    "name": "Tomato",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  },
                  {
                    "id": "5a67f531a4227a2fac230c8e",
                    "name": "Balanced U",
                    "type": "label"
                  }
                ],
                "id": "5af7338617584bbc736d55c4",
                "ingredients": "Tomatoes Cherry Fresh",
                "mrn": "62343",
                "mrn_full": "62343.0",
                "name": "Cherry Tomatoes",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061c68",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "5",
                    "value_numeric": "5"
                  },
                  {
                    "id": "5d23f9594198d409c3061c69",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c6a",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c6b",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c6c",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c6d",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c6e",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c6f",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061c70",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "1",
                    "value_numeric": "1"
                  },
                  {
                    "id": "5d23f9594198d409c3061c71",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c72",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c73",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "1 ounce",
                "qty": null,
                "rev": "0",
                "sort_order": 10,
                "webtrition_id": 106456750
              },
              {
                "calories": 45,
                "custom_allergens": [],
                "desc": "Garbanzo Beans",
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  }
                ],
                "id": "59e3caf828d0e73e15f77781",
                "ingredients": "Beans Garbanzo Canned Drained Rinsed",
                "mrn": "47685",
                "mrn_full": "47685.0",
                "name": "Garbanzo Beans",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061c74",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "45",
                    "value_numeric": "45"
                  },
                  {
                    "id": "5d23f9594198d409c3061c75",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "5",
                    "value_numeric": "5"
                  },
                  {
                    "id": "5d23f9594198d409c3061c76",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c77",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "2",
                    "value_numeric": "2"
                  },
                  {
                    "id": "5d23f9594198d409c3061c78",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "3",
                    "value_numeric": "3"
                  },
                  {
                    "id": "5d23f9594198d409c3061c79",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c7a",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "70",
                    "value_numeric": "70"
                  },
                  {
                    "id": "5d23f9594198d409c3061c7b",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "1",
                    "value_numeric": "1"
                  },
                  {
                    "id": "5d23f9594198d409c3061c7c",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "8",
                    "value_numeric": "8"
                  },
                  {
                    "id": "5d23f9594198d409c3061c7d",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0.5",
                    "value_numeric": "0.5"
                  },
                  {
                    "id": "5d23f9594198d409c3061c7e",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c7f",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "1 ounce",
                "qty": null,
                "rev": "0",
                "sort_order": 11,
                "webtrition_id": 106456792
              },
              {
                "calories": 0,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  }
                ],
                "id": "5c2fb62adc5b76af72fa4f01",
                "ingredients": "Carrots Fresh Grated",
                "mrn": "47708",
                "mrn_full": "47708.0",
                "name": "Fresh Carrots",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061c80",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c81",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c82",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c83",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c84",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c85",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c86",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c87",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c88",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061c89",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c8a",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c8b",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "1 tbsp",
                "qty": null,
                "rev": "0",
                "sort_order": 12,
                "webtrition_id": 106456804
              },
              {
                "calories": 10,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fcf",
                    "name": "Onion",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  },
                  {
                    "id": "5a67f531a4227a2fac230c8e",
                    "name": "Balanced U",
                    "type": "label"
                  }
                ],
                "id": "5af5761117584bbc736d52ab",
                "ingredients": "Onions Red Fresh Each Slice",
                "mrn": "14918",
                "mrn_full": "14918.0",
                "name": "Red Onion Slice",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061c8c",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "10",
                    "value_numeric": "10"
                  },
                  {
                    "id": "5d23f9594198d409c3061c8d",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c8e",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c8f",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c90",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c91",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c92",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c93",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "1",
                    "value_numeric": "1"
                  },
                  {
                    "id": "5d23f9594198d409c3061c94",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "3",
                    "value_numeric": "3"
                  },
                  {
                    "id": "5d23f9594198d409c3061c95",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c96",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c97",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "1 ounce",
                "qty": null,
                "rev": "0",
                "sort_order": 13,
                "webtrition_id": 106456747
              },
              {
                "calories": 5,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  },
                  {
                    "id": "5934c5773191a24f12b53121",
                    "name": "Mushroom",
                    "type": "allergen"
                  },
                  {
                    "id": "5a67f531a4227a2fac230c8e",
                    "name": "Balanced U",
                    "type": "label"
                  }
                ],
                "id": "5af4f42117584bbc736d5026",
                "ingredients": "Mushrooms Button Fresh Sliced",
                "mrn": "62338",
                "mrn_full": "62338.0",
                "name": "Sliced Mushrooms",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061c98",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "5",
                    "value_numeric": "5"
                  },
                  {
                    "id": "5d23f9594198d409c3061c99",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c9a",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c9b",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c9c",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061c9d",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c9e",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061c9f",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061ca0",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061ca1",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061ca2",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061ca3",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "1 ounce",
                "qty": null,
                "rev": "0",
                "sort_order": 14,
                "webtrition_id": 106456765
              },
              {
                "calories": 70,
                "custom_allergens": [],
                "desc": "Croutons to add to a salad",
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  },
                  {
                    "id": "5934c5733191a24f12b52fdf",
                    "name": "Gluten",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe2",
                    "name": "Wheat",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff2",
                    "name": "Garlic",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b53002",
                    "name": "Soy",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c576ee596f19f2126a72",
                    "name": "Milk*",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c577ee596f19f2126aa5",
                    "name": "Tree Nuts*",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c57aee596f19f2126bbd",
                    "name": "Peanuts*",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c742ee596f19fb110726",
                    "name": "Egg*",
                    "type": "allergen"
                  }
                ],
                "id": "5b222bdaefeb90a78e92135a",
                "ingredients": "Bread French Baguette Parbaked 22\". 10.5 oz, Garlic Cloves Peeled Fresh Minced, Salt Kosher, Oil Canola",
                "mrn": "31698",
                "mrn_full": "31698.1",
                "name": "Croutons",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061ca4",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "70",
                    "value_numeric": "70"
                  },
                  {
                    "id": "5d23f9594198d409c3061ca5",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "5",
                    "value_numeric": "5"
                  },
                  {
                    "id": "5d23f9594198d409c3061ca6",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061ca7",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061ca8",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "3",
                    "value_numeric": "3"
                  },
                  {
                    "id": "5d23f9594198d409c3061ca9",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061caa",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "340",
                    "value_numeric": "340"
                  },
                  {
                    "id": "5d23f9594198d409c3061cab",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "1",
                    "value_numeric": "1"
                  },
                  {
                    "id": "5d23f9594198d409c3061cac",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "14",
                    "value_numeric": "14"
                  },
                  {
                    "id": "5d23f9594198d409c3061cad",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0.5",
                    "value_numeric": "0.5"
                  },
                  {
                    "id": "5d23f9594198d409c3061cae",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061caf",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "1 ounce",
                "qty": null,
                "rev": "1",
                "sort_order": 15,
                "webtrition_id": 106456795
              },
              {
                "calories": 15,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  }
                ],
                "id": "59e3fbd328d0e73e15f7bf68",
                "ingredients": "Seeds Sunflower Roasted Unsalted",
                "mrn": "47803",
                "mrn_full": "47803.0",
                "name": "Sunflower Seeds",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061cb0",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "15",
                    "value_numeric": "15"
                  },
                  {
                    "id": "5d23f9594198d409c3061cb1",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "10",
                    "value_numeric": "10"
                  },
                  {
                    "id": "5d23f9594198d409c3061cb2",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061cb3",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061cb4",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061cb5",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061cb6",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061cb7",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061cb8",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061cb9",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "1.5",
                    "value_numeric": "1.5"
                  },
                  {
                    "id": "5d23f9594198d409c3061cba",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "-",
                    "value_numeric": "-"
                  },
                  {
                    "id": "5d23f9594198d409c3061cbb",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "1 tsp",
                "qty": null,
                "rev": "0",
                "sort_order": 16,
                "webtrition_id": 106456798
              },
              {
                "calories": 30,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  }
                ],
                "id": "5b92e695dc5b76af72f9d428",
                "ingredients": "Cranberries Dried",
                "mrn": "47784",
                "mrn_full": "47784.0",
                "name": "Dried Cranberries",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061cbc",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "30",
                    "value_numeric": "30"
                  },
                  {
                    "id": "5d23f9594198d409c3061cbd",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061cbe",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061cbf",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061cc0",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061cc1",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061cc2",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061cc3",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "7",
                    "value_numeric": "7"
                  },
                  {
                    "id": "5d23f9594198d409c3061cc4",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "8",
                    "value_numeric": "8"
                  },
                  {
                    "id": "5d23f9594198d409c3061cc5",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061cc6",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061cc7",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "1 tbsp",
                "qty": null,
                "rev": "0",
                "sort_order": 17,
                "webtrition_id": 106456801
              },
              {
                "calories": 110,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fcf",
                    "name": "Onion",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe0",
                    "name": "Milk",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff1",
                    "name": "Egg",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff2",
                    "name": "Garlic",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff3",
                    "name": "Mustard*",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b53002",
                    "name": "Soy",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c57aee596f19f2126c06",
                    "name": "Gluten*",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c580ee596f19f2126dea",
                    "name": "MSG",
                    "type": "allergen"
                  }
                ],
                "id": "5ca4c97ee67a2d1b3b8dfec9",
                "ingredients": "Mayonnaise Hellman's Heavy Duty, Milk Buttermilk Low Fat 1%, Mix Salad Dressing Ranch",
                "mrn": "104930",
                "mrn_full": "104930.0",
                "name": "Ranch Dressing",
                "nutrients": [
                  {
                    "id": "5d23f9594198d409c3061cc8",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "110",
                    "value_numeric": "110"
                  },
                  {
                    "id": "5d23f9594198d409c3061cc9",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "100",
                    "value_numeric": "100"
                  },
                  {
                    "id": "5d23f9594198d409c3061cca",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "10",
                    "value_numeric": "10"
                  },
                  {
                    "id": "5d23f9594198d409c3061ccb",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f9594198d409c3061ccc",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061ccd",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "1.5",
                    "value_numeric": "1.5"
                  },
                  {
                    "id": "5d23f9594198d409c3061cce",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "230",
                    "value_numeric": "230"
                  },
                  {
                    "id": "5d23f9594198d409c3061ccf",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f9594198d409c3061cd0",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "1",
                    "value_numeric": "1"
                  },
                  {
                    "id": "5d23f9594198d409c3061cd1",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "11",
                    "value_numeric": "11"
                  },
                  {
                    "id": "5d23f9594198d409c3061cd2",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "-",
                    "value_numeric": "-"
                  },
                  {
                    "id": "5d23f9594198d409c3061cd3",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0+",
                    "value_numeric": "0+"
                  }
                ],
                "portion": "2 tbsp",
                "qty": null,
                "rev": "0",
                "sort_order": 18,
                "webtrition_id": 106456783
              },
              {
                "calories": 160,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd0",
                    "name": "Sulphites",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff2",
                    "name": "Garlic",
                    "type": "allergen"
                  }
                ],
                "id": "5cd4bd24e67a2d1b3b8214d1",
                "ingredients": "Oil Canola, Vinegar Red Wine, Garlic Cloves Peeled Fresh Chopped, Spice Oregano Dried Crushed, Sugar Granulated, Salt Kosher, Spice Pepper Black Ground",
                "mrn": "75891",
                "mrn_full": "75891.0",
                "name": "Garlic Vinaigrette",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061cd4",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "160",
                    "value_numeric": "160"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cd5",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "160",
                    "value_numeric": "160"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cd6",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0+",
                    "value_numeric": "0+"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cd7",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cd8",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cd9",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "1.5",
                    "value_numeric": "1.5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cda",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "30",
                    "value_numeric": "30"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cdb",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cdc",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cdd",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "18",
                    "value_numeric": "18"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cde",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "-",
                    "value_numeric": "-"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cdf",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0+",
                    "value_numeric": "0+"
                  }
                ],
                "portion": "1 floz",
                "qty": null,
                "rev": "0",
                "sort_order": 19,
                "webtrition_id": 106456729
              },
              {
                "calories": 30,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fcf",
                    "name": "Onion",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff2",
                    "name": "Garlic",
                    "type": "allergen"
                  }
                ],
                "id": "59efa36c28d0e73e15f87f38",
                "ingredients": "Salad Dressing Raspberry Fat Free Bulk",
                "mrn": "16719",
                "mrn_full": "16719.0",
                "name": "Fat Free Raspberry Dressing",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061ce0",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "30",
                    "value_numeric": "30"
                  },
                  {
                    "id": "5d23f95a4198d409c3061ce1",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061ce2",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061ce3",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061ce4",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061ce5",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061ce6",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "270",
                    "value_numeric": "270"
                  },
                  {
                    "id": "5d23f95a4198d409c3061ce7",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "6",
                    "value_numeric": "6"
                  },
                  {
                    "id": "5d23f95a4198d409c3061ce8",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "6",
                    "value_numeric": "6"
                  },
                  {
                    "id": "5d23f95a4198d409c3061ce9",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cea",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061ceb",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "-",
                    "value_numeric": "-"
                  }
                ],
                "portion": "1 floz",
                "qty": null,
                "rev": "0",
                "sort_order": 20,
                "webtrition_id": 106456780
              },
              {
                "calories": 110,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fcf",
                    "name": "Onion",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe0",
                    "name": "Milk",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff0",
                    "name": "Celery",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff1",
                    "name": "Egg",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff2",
                    "name": "Garlic",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff3",
                    "name": "Mustard*",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b53002",
                    "name": "Soy",
                    "type": "allergen"
                  }
                ],
                "id": "5b6b21dcdc5b76af72f98d91",
                "ingredients": "Salad Dressing Caesar Creamy",
                "mrn": "44327",
                "mrn_full": "44327.0",
                "name": "Caesar Dressing",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061cec",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "110",
                    "value_numeric": "110"
                  },
                  {
                    "id": "5d23f95a4198d409c3061ced",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "100",
                    "value_numeric": "100"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cee",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "10",
                    "value_numeric": "10"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cef",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cf0",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "1",
                    "value_numeric": "1"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cf1",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "2",
                    "value_numeric": "2"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cf2",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "310",
                    "value_numeric": "310"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cf3",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "1",
                    "value_numeric": "1"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cf4",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "2",
                    "value_numeric": "2"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cf5",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "11",
                    "value_numeric": "11"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cf6",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cf7",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "-",
                    "value_numeric": "-"
                  }
                ],
                "portion": "1 floz",
                "qty": null,
                "rev": "0",
                "sort_order": 21,
                "webtrition_id": 106456786
              },
              {
                "calories": 110,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5733191a24f12b52fdf",
                    "name": "Gluten",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe2",
                    "name": "Wheat",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff2",
                    "name": "Garlic",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff3",
                    "name": "Mustard*",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b53002",
                    "name": "Soy",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c580ee596f19fb110473",
                    "name": "Sesame Seeds",
                    "type": "allergen"
                  }
                ],
                "id": "59ef7dfc28d0e73e15f87d84",
                "ingredients": "Salad Dressing Sesame Bulk",
                "mrn": "16689",
                "mrn_full": "16689.0",
                "name": "Sesame Dressing",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061cf8",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "110",
                    "value_numeric": "110"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cf9",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "80",
                    "value_numeric": "80"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cfa",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cfb",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cfc",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cfd",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "1.5",
                    "value_numeric": "1.5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cfe",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "280",
                    "value_numeric": "280"
                  },
                  {
                    "id": "5d23f95a4198d409c3061cff",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "6",
                    "value_numeric": "6"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d00",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "6",
                    "value_numeric": "6"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d01",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "9",
                    "value_numeric": "9"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d02",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d03",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "-",
                    "value_numeric": "-"
                  }
                ],
                "portion": "1 floz",
                "qty": null,
                "rev": "0",
                "sort_order": 22,
                "webtrition_id": 106456789
              },
              {
                "calories": 15,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fcf",
                    "name": "Onion",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe0",
                    "name": "Milk",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff2",
                    "name": "Garlic",
                    "type": "allergen"
                  }
                ],
                "id": "59eb5cf728d0e73e15f85b16",
                "ingredients": "Salad Dressing Italian Fat Free Bulk",
                "mrn": "62355",
                "mrn_full": "62355.0",
                "name": "Fat Free Italian Dressing",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061d04",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "15",
                    "value_numeric": "15"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d05",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d06",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d07",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d08",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d09",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d0a",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "190",
                    "value_numeric": "190"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d0b",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "2",
                    "value_numeric": "2"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d0c",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "3",
                    "value_numeric": "3"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d0d",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d0e",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d0f",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "1 floz",
                "qty": null,
                "rev": "0",
                "sort_order": 23,
                "webtrition_id": 106456777
              },
              {
                "calories": 70,
                "custom_allergens": [],
                "desc": "With a touch of clover honey and tangy mustard",
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5733191a24f12b52fef",
                    "name": "Alcohol",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff1",
                    "name": "Egg",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b53002",
                    "name": "Soy",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5743191a24f12b53029",
                    "name": "Mustard",
                    "type": "allergen"
                  }
                ],
                "id": "59fad17528d0e73e15f8abc6",
                "ingredients": "Salad Dressing Honey Mustard Bulk",
                "mrn": "5323",
                "mrn_full": "5323.0",
                "name": "Honey Mustard Dressing",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061d10",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "70",
                    "value_numeric": "70"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d11",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "45",
                    "value_numeric": "45"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d12",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d13",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d14",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d15",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d16",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "190",
                    "value_numeric": "190"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d17",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "4",
                    "value_numeric": "4"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d18",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "5",
                    "value_numeric": "5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d19",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "5",
                    "value_numeric": "5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d1a",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d1b",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "1 floz",
                "qty": null,
                "rev": "0",
                "sort_order": 24,
                "webtrition_id": 106456731
              },
              {
                "calories": 240,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  }
                ],
                "id": "5aad49d4d731be9fb4cc155a",
                "ingredients": "Oil Olive Extra Virgin",
                "mrn": "63338",
                "mrn_full": "63338.2",
                "name": "Extra Virgin Olive Oil",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061d1c",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "240",
                    "value_numeric": "240"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d1d",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "240",
                    "value_numeric": "240"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d1e",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d1f",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d20",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d21",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "3.5",
                    "value_numeric": "3.5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d22",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d23",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d24",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d25",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "27",
                    "value_numeric": "27"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d26",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "-",
                    "value_numeric": "-"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d27",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "1 floz",
                "qty": null,
                "rev": "2",
                "sort_order": 25,
                "webtrition_id": 106456733
              },
              {
                "calories": 15,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd0",
                    "name": "Sulphites",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  }
                ],
                "id": "59e3fa1828d0e73e15f7bc19",
                "ingredients": "Vinegar Balsamic",
                "mrn": "47957",
                "mrn_full": "47957.11",
                "name": "Balsamic Vinegar",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061d28",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "15",
                    "value_numeric": "15"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d29",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d2a",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "-",
                    "value_numeric": "-"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d2b",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "-",
                    "value_numeric": "-"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d2c",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d2d",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d2e",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d2f",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "2",
                    "value_numeric": "2"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d30",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "3",
                    "value_numeric": "3"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d31",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d32",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d33",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "-",
                    "value_numeric": "-"
                  }
                ],
                "portion": "1/2 floz",
                "qty": null,
                "rev": "11",
                "sort_order": 26,
                "webtrition_id": 106456735
              },
              {
                "calories": 0,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd0",
                    "name": "Sulphites",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  }
                ],
                "id": "59e3fa1828d0e73e15f7bc1d",
                "ingredients": "Vinegar Red Wine",
                "mrn": "47957",
                "mrn_full": "47957.1",
                "name": "Red Wine Vinegar ",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061d34",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d35",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d36",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "-",
                    "value_numeric": "-"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d37",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d38",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d39",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d3a",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d3b",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d3c",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d3d",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d3e",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d3f",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "-",
                    "value_numeric": "-"
                  }
                ],
                "portion": "1/2 floz",
                "qty": null,
                "rev": "1",
                "sort_order": 27,
                "webtrition_id": 106456738
              }
            ],
            "name": "Salad Bar",
            "sort_order": 5
          },
          {
            "id": "5d23f9384198d409c306186f",
            "items": [
              {
                "calories": 230,
                "custom_allergens": [],
                "desc": "Whole Wheat Kaiser Bun",
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5733191a24f12b52fdf",
                    "name": "Gluten",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe0",
                    "name": "Milk",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe2",
                    "name": "Wheat",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b53002",
                    "name": "Soy",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c580ee596f19fb110473",
                    "name": "Sesame Seeds",
                    "type": "allergen"
                  }
                ],
                "id": "59e3cff728d0e73e15f77f43",
                "ingredients": "Roll Deli Whole Wheat 3 oz",
                "mrn": "50748",
                "mrn_full": "50748.3",
                "name": "Whole Wheat Kaiser Bun",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061d40",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "230",
                    "value_numeric": "230"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d41",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "35",
                    "value_numeric": "35"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d42",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d43",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "6",
                    "value_numeric": "6"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d44",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "7",
                    "value_numeric": "7"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d45",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0.5",
                    "value_numeric": "0.5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d46",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "440",
                    "value_numeric": "440"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d47",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "7",
                    "value_numeric": "7"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d48",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "43",
                    "value_numeric": "43"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d49",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "4",
                    "value_numeric": "4"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d4a",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "-",
                    "value_numeric": "-"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d4b",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "1 each",
                "qty": null,
                "rev": "3",
                "sort_order": 1,
                "webtrition_id": 106457375
              },
              {
                "calories": 190,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5733191a24f12b52fdf",
                    "name": "Gluten",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe0",
                    "name": "Milk",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe2",
                    "name": "Wheat",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b53002",
                    "name": "Soy",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c577ee596f19f2126aa5",
                    "name": "Tree Nuts*",
                    "type": "allergen"
                  }
                ],
                "id": "59e3cff728d0e73e15f77f44",
                "ingredients": "Bread Healthy Choice 7-grain Slice 1.34 oz",
                "mrn": "48147",
                "mrn_full": "48147.0",
                "name": "Multigrain Bread",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061d4c",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "190",
                    "value_numeric": "190"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d4d",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "15",
                    "value_numeric": "15"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d4e",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d4f",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "5",
                    "value_numeric": "5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d50",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "9",
                    "value_numeric": "9"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d51",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d52",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "300",
                    "value_numeric": "300"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d53",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "8",
                    "value_numeric": "8"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d54",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "37",
                    "value_numeric": "37"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d55",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "1.5",
                    "value_numeric": "1.5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d56",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "1",
                    "value_numeric": "1"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d57",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "2 slice",
                "qty": null,
                "rev": "0",
                "sort_order": 2,
                "webtrition_id": 106457369
              },
              {
                "calories": 130,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5733191a24f12b52fdf",
                    "name": "Gluten",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe2",
                    "name": "Wheat",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b53002",
                    "name": "Soy",
                    "type": "allergen"
                  },
                  {
                    "id": "5a67f531a4227a2fac230c8e",
                    "name": "Balanced U",
                    "type": "label"
                  }
                ],
                "id": "59e3ca6028d0e73e15f7763a",
                "ingredients": "Bread Whole Wheat Slice .88 oz",
                "mrn": "1390",
                "mrn_full": "1390.0",
                "name": "Whole Wheat Bread",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061d58",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "130",
                    "value_numeric": "130"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d59",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "15",
                    "value_numeric": "15"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d5a",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d5b",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "3",
                    "value_numeric": "3"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d5c",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "6",
                    "value_numeric": "6"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d5d",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d5e",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "230",
                    "value_numeric": "230"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d5f",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "2",
                    "value_numeric": "2"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d60",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "21",
                    "value_numeric": "21"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d61",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "1.5",
                    "value_numeric": "1.5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d62",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d63",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "2 slice",
                "qty": null,
                "rev": "0",
                "sort_order": 3,
                "webtrition_id": 106457370
              },
              {
                "calories": 160,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  },
                  {
                    "id": "5934c5733191a24f12b52fdf",
                    "name": "Gluten",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe2",
                    "name": "Wheat",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b53002",
                    "name": "Soy",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c577ee596f19f2126aa5",
                    "name": "Tree Nuts*",
                    "type": "allergen"
                  }
                ],
                "id": "59e3caf828d0e73e15f77757",
                "ingredients": "Bread White Slice 1.08 oz",
                "mrn": "1251",
                "mrn_full": "1251.0",
                "name": "White Bread",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061d64",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "160",
                    "value_numeric": "160"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d65",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "20",
                    "value_numeric": "20"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d66",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d67",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "2",
                    "value_numeric": "2"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d68",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "5",
                    "value_numeric": "5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d69",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d6a",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "300",
                    "value_numeric": "300"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d6b",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "3",
                    "value_numeric": "3"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d6c",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "30",
                    "value_numeric": "30"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d6d",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "2",
                    "value_numeric": "2"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d6e",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d6f",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "2 slice",
                "qty": null,
                "rev": "0",
                "sort_order": 4,
                "webtrition_id": 106457376
              },
              {
                "calories": 320,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd0",
                    "name": "Sulphites",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  },
                  {
                    "id": "5934c5733191a24f12b52fdf",
                    "name": "Gluten",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe2",
                    "name": "Wheat",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b53002",
                    "name": "Soy",
                    "type": "allergen"
                  }
                ],
                "id": "59e3cf9a28d0e73e15f77d4c",
                "ingredients": "Tortilla Flour Heat Pressed 12\"",
                "mrn": "62283",
                "mrn_full": "62283.0",
                "name": "Flour Toritlla, 12\"",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061d70",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "320",
                    "value_numeric": "320"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d71",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "70",
                    "value_numeric": "70"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d72",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d73",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "4",
                    "value_numeric": "4"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d74",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "9",
                    "value_numeric": "9"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d75",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "3",
                    "value_numeric": "3"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d76",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "770",
                    "value_numeric": "770"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d77",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "4",
                    "value_numeric": "4"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d78",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "51",
                    "value_numeric": "51"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d79",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "8",
                    "value_numeric": "8"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d7a",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d7b",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "1 each",
                "qty": null,
                "rev": "0",
                "sort_order": 6,
                "webtrition_id": 106457373
              },
              {
                "calories": 90,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5733191a24f12b52fe0",
                    "name": "Milk",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5753191a24f12b5305b",
                    "name": "MSG*",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c576ee596f19f2126a40",
                    "name": "Poultry",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c57aee596f19f2126c06",
                    "name": "Gluten*",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c57aee596f19f2126c07",
                    "name": "Wheat*",
                    "type": "allergen"
                  }
                ],
                "id": "59e3cff728d0e73e15f77f49",
                "ingredients": "Turkey Breast Deli Sliced Thin",
                "mrn": "48144",
                "mrn_full": "48144.1",
                "name": "Thinly Sliced Deli Turkey Breast",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061d7c",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "90",
                    "value_numeric": "90"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d7d",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "30",
                    "value_numeric": "30"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d7e",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "40",
                    "value_numeric": "40"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d7f",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d80",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "11",
                    "value_numeric": "11"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d81",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "1",
                    "value_numeric": "1"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d82",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "770",
                    "value_numeric": "770"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d83",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d84",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "3",
                    "value_numeric": "3"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d85",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "3.5",
                    "value_numeric": "3.5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d86",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d87",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "5",
                    "value_numeric": "5"
                  }
                ],
                "portion": "3 ounce",
                "qty": null,
                "rev": "1",
                "sort_order": 7,
                "webtrition_id": 106457360
              },
              {
                "calories": 110,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5733191a24f12b52ff4",
                    "name": "Pork",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c57aee596f19f2126c06",
                    "name": "Gluten*",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c57aee596f19f2126c07",
                    "name": "Wheat*",
                    "type": "allergen"
                  }
                ],
                "id": "59e3cff728d0e73e15f77f4a",
                "ingredients": "Pork Ham Buffet Boneless Smoked Sliced Thin",
                "mrn": "14910",
                "mrn_full": "14910.0",
                "name": "Thinly Sliced Smoked Ham",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061d88",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "110",
                    "value_numeric": "110"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d89",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "40",
                    "value_numeric": "40"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d8a",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "45",
                    "value_numeric": "45"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d8b",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d8c",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "15",
                    "value_numeric": "15"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d8d",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "1.5",
                    "value_numeric": "1.5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d8e",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "1000",
                    "value_numeric": "1000"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d8f",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "1",
                    "value_numeric": "1"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d90",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "1",
                    "value_numeric": "1"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d91",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "4.5",
                    "value_numeric": "4.5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d92",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d93",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "25",
                    "value_numeric": "25"
                  }
                ],
                "portion": "3 ounce",
                "qty": null,
                "rev": "0",
                "sort_order": 8,
                "webtrition_id": 106457368
              },
              {
                "calories": 290,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5733191a24f12b52ff2",
                    "name": "Garlic",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff3",
                    "name": "Mustard*",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff4",
                    "name": "Pork",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5763191a24f12b530b1",
                    "name": "Beef",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c576ee596f19f2126a72",
                    "name": "Milk*",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c57bee596f19f2126c69",
                    "name": "Celery*",
                    "type": "allergen"
                  }
                ],
                "id": "5ab28177d731be9fb4cc1945",
                "ingredients": "Salami Genoa Sliced 1 oz",
                "mrn": "48144",
                "mrn_full": "48144.27",
                "name": "Sliced Genoa Salami",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061d94",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "290",
                    "value_numeric": "290"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d95",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "200",
                    "value_numeric": "200"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d96",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "75",
                    "value_numeric": "75"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d97",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d98",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "19",
                    "value_numeric": "19"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d99",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "8",
                    "value_numeric": "8"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d9a",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "1480",
                    "value_numeric": "1480"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d9b",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d9c",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "2",
                    "value_numeric": "2"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d9d",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "22",
                    "value_numeric": "22"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d9e",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061d9f",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "35",
                    "value_numeric": "35"
                  }
                ],
                "portion": "3 ounce",
                "qty": null,
                "rev": "27",
                "sort_order": 9,
                "webtrition_id": 106457361
              },
              {
                "calories": 90,
                "custom_allergens": [],
                "desc": "Classic tuna salad ",
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fcf",
                    "name": "Onion",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff0",
                    "name": "Celery",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff1",
                    "name": "Egg",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b53002",
                    "name": "Soy",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5743191a24f12b53029",
                    "name": "Mustard",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5753191a24f12b5305b",
                    "name": "MSG*",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c577ee596f19f2126aa4",
                    "name": "Fish",
                    "type": "allergen"
                  },
                  {
                    "id": "5a67f531a4227a2fac230c8e",
                    "name": "Balanced U",
                    "type": "label"
                  }
                ],
                "id": "59e3caf828d0e73e15f77756",
                "ingredients": "Fish Tuna Chunk Light FAD Free Water Packed, Oil Canola, Onions Red Fresh Chopped Fine, Celery Fresh Chopped Fine, Juice Lemon Fresh, Mayonnaise Light Kraft, Salt Kosher, Spice Pepper Black Ground",
                "mrn": "12043",
                "mrn_full": "12043.5",
                "name": "FIT Tuna Salad",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061da0",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "90",
                    "value_numeric": "90"
                  },
                  {
                    "id": "5d23f95a4198d409c3061da1",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "50",
                    "value_numeric": "50"
                  },
                  {
                    "id": "5d23f95a4198d409c3061da2",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "15",
                    "value_numeric": "15"
                  },
                  {
                    "id": "5d23f95a4198d409c3061da3",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061da4",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "8",
                    "value_numeric": "8"
                  },
                  {
                    "id": "5d23f95a4198d409c3061da5",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0.5",
                    "value_numeric": "0.5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061da6",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "240",
                    "value_numeric": "240"
                  },
                  {
                    "id": "5d23f95a4198d409c3061da7",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061da8",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f95a4198d409c3061da9",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "6",
                    "value_numeric": "6"
                  },
                  {
                    "id": "5d23f95a4198d409c3061daa",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dab",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "20+",
                    "value_numeric": "20+"
                  }
                ],
                "portion": "3 ounce",
                "qty": null,
                "rev": "5",
                "sort_order": 10,
                "webtrition_id": 106457377
              },
              {
                "calories": 100,
                "custom_allergens": [],
                "desc": "Rich and creamy",
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff2",
                    "name": "Garlic",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c580ee596f19fb110473",
                    "name": "Sesame Seeds",
                    "type": "allergen"
                  },
                  {
                    "id": "5a67f531a4227a2fac230c8e",
                    "name": "Balanced U",
                    "type": "label"
                  }
                ],
                "id": "59e3febf28d0e73e15f7c4fe",
                "ingredients": "Beans Garbanzo Canned Drained Rinsed, Water, Paste Sesame Tahini, Juice Lemon Fresh, Spice Cumin Ground, Garlic Cloves Peeled Fresh Chopped, Salt Kosher",
                "mrn": "24644",
                "mrn_full": "24644.5",
                "name": "Classic Hummus",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061dac",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "100",
                    "value_numeric": "100"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dad",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "30",
                    "value_numeric": "30"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dae",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061daf",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "4",
                    "value_numeric": "4"
                  },
                  {
                    "id": "5d23f95a4198d409c3061db0",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "5",
                    "value_numeric": "5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061db1",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061db2",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "150",
                    "value_numeric": "150"
                  },
                  {
                    "id": "5d23f95a4198d409c3061db3",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "2",
                    "value_numeric": "2"
                  },
                  {
                    "id": "5d23f95a4198d409c3061db4",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "13",
                    "value_numeric": "13"
                  },
                  {
                    "id": "5d23f95a4198d409c3061db5",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "3.5",
                    "value_numeric": "3.5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061db6",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "-",
                    "value_numeric": "-"
                  },
                  {
                    "id": "5d23f95a4198d409c3061db7",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "2 ounce",
                "qty": null,
                "rev": "5",
                "sort_order": 11,
                "webtrition_id": 106457357
              },
              {
                "calories": 50,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe0",
                    "name": "Milk",
                    "type": "allergen"
                  },
                  {
                    "id": "5a67f531a4227a2fac230c8e",
                    "name": "Balanced U",
                    "type": "label"
                  }
                ],
                "id": "59e3d6dc28d0e73e15f78a77",
                "ingredients": "Cheese American Sliced .5 oz",
                "mrn": "1748",
                "mrn_full": "1748.0",
                "name": "American Cheese Slice",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061db8",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "50",
                    "value_numeric": "50"
                  },
                  {
                    "id": "5d23f95a4198d409c3061db9",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "40",
                    "value_numeric": "40"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dba",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "15",
                    "value_numeric": "15"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dbb",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dbc",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "3",
                    "value_numeric": "3"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dbd",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "2.5",
                    "value_numeric": "2.5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dbe",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "240",
                    "value_numeric": "240"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dbf",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dc0",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dc1",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "4.5",
                    "value_numeric": "4.5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dc2",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dc3",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "45",
                    "value_numeric": "45"
                  }
                ],
                "portion": "1 slice",
                "qty": null,
                "rev": "0",
                "sort_order": 12,
                "webtrition_id": 106457362
              },
              {
                "calories": 60,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe0",
                    "name": "Milk",
                    "type": "allergen"
                  }
                ],
                "id": "59e3febf28d0e73e15f7c500",
                "ingredients": "Cheese Cheddar Mild Loaf .5 oz Sliced",
                "mrn": "43037",
                "mrn_full": "43037.1",
                "name": "Cheddar Cheese Slice",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061dc4",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "60",
                    "value_numeric": "60"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dc5",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "40",
                    "value_numeric": "40"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dc6",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "15",
                    "value_numeric": "15"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dc7",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dc8",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "3",
                    "value_numeric": "3"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dc9",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "2.5",
                    "value_numeric": "2.5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dca",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "95",
                    "value_numeric": "95"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dcb",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dcc",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dcd",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "4.5",
                    "value_numeric": "4.5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dce",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dcf",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "5",
                    "value_numeric": "5"
                  }
                ],
                "portion": "1 slice",
                "qty": null,
                "rev": "1",
                "sort_order": 13,
                "webtrition_id": 106457374
              },
              {
                "calories": 100,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5733191a24f12b52fe0",
                    "name": "Milk",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b53002",
                    "name": "Soy",
                    "type": "allergen"
                  }
                ],
                "id": "59e3febf28d0e73e15f7c4fd",
                "ingredients": "Cheese American Swiss Sliced 0.5 oz",
                "mrn": "43034",
                "mrn_full": "43034.1",
                "name": "Sliced American Swiss Cheese",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061dd0",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "100",
                    "value_numeric": "100"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dd1",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "80",
                    "value_numeric": "80"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dd2",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "30",
                    "value_numeric": "30"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dd3",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dd4",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "5",
                    "value_numeric": "5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dd5",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "5",
                    "value_numeric": "5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dd6",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "470",
                    "value_numeric": "470"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dd7",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dd8",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "1",
                    "value_numeric": "1"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dd9",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "9",
                    "value_numeric": "9"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dda",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061ddb",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "90",
                    "value_numeric": "90"
                  }
                ],
                "portion": "1 slice",
                "qty": null,
                "rev": "1",
                "sort_order": 14,
                "webtrition_id": 106457372
              },
              {
                "calories": 0,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  },
                  {
                    "id": "5a67f531a4227a2fac230c8e",
                    "name": "Balanced U",
                    "type": "label"
                  }
                ],
                "id": "5c589c5bdc5b76af72fa8aea",
                "ingredients": "Cucumbers Fresh Scored Sliced Thin Each Slice",
                "mrn": "68562",
                "mrn_full": "68562.0",
                "name": "Sliced Cucumber",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061ddc",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061ddd",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dde",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061ddf",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061de0",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061de1",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061de2",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061de3",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061de4",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "1",
                    "value_numeric": "1"
                  },
                  {
                    "id": "5d23f95a4198d409c3061de5",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061de6",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061de7",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "1 ounce",
                "qty": null,
                "rev": "0",
                "sort_order": 15,
                "webtrition_id": 106457367
              },
              {
                "calories": 5,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  },
                  {
                    "id": "5a67f531a4227a2fac230c8e",
                    "name": "Balanced U",
                    "type": "label"
                  }
                ],
                "id": "5af4f5a117584bbc736d503e",
                "ingredients": "Peppers Bell Green Fresh Sliced",
                "mrn": "62342",
                "mrn_full": "62342.0",
                "name": "Sliced Green Bell Pepper",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061de8",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "5",
                    "value_numeric": "5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061de9",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dea",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061deb",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dec",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061ded",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dee",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061def",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f95a4198d409c3061df0",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "1",
                    "value_numeric": "1"
                  },
                  {
                    "id": "5d23f95a4198d409c3061df1",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061df2",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061df3",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "1 ounce",
                "qty": null,
                "rev": "0",
                "sort_order": 16,
                "webtrition_id": 106457363
              },
              {
                "calories": 0,
                "custom_allergens": [],
                "desc": null,
                "filters": [
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
                "id": "59e3caf828d0e73e15f7776f",
                "ingredients": "Pickles Dill Hamburger Slices",
                "mrn": "63438",
                "mrn_full": "63438.0",
                "name": "Dill Pickle Slices",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061df4",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061df5",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061df6",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061df7",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061df8",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061df9",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dfa",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "115",
                    "value_numeric": "115"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dfb",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dfc",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dfd",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dfe",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061dff",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "2 each",
                "qty": null,
                "rev": "0",
                "sort_order": 17,
                "webtrition_id": 106457365
              },
              {
                "calories": 0,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff2",
                    "name": "Garlic",
                    "type": "allergen"
                  }
                ],
                "id": "59e3d34f28d0e73e15f785f6",
                "ingredients": "Peppers Chili Jalapeno Sliced Canned",
                "mrn": "13404",
                "mrn_full": "13404.4",
                "name": "Sliced Jalapeno Pepper",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061e00",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e01",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e02",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e03",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e04",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e05",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e06",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "250",
                    "value_numeric": "250"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e07",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e08",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e09",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e0a",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e0b",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "1 tbsp",
                "qty": null,
                "rev": "4",
                "sort_order": 18,
                "webtrition_id": 106457378
              },
              {
                "calories": 0,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  },
                  {
                    "id": "5a67f531a4227a2fac230c8e",
                    "name": "Balanced U",
                    "type": "label"
                  }
                ],
                "id": "5af4efc017584bbc736d4fe2",
                "ingredients": "Lettuce Leaf Individual Leaf Fresh",
                "mrn": "14957",
                "mrn_full": "14957.0",
                "name": "Lettuce Leaf",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061e0c",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e0d",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e0e",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e0f",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e10",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e11",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e12",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e13",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e14",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e15",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e16",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e17",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "1 each",
                "qty": null,
                "rev": "0",
                "sort_order": 19,
                "webtrition_id": 106457366
              },
              {
                "calories": 0,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd1",
                    "name": "Tomato",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  },
                  {
                    "id": "5a67f531a4227a2fac230c8e",
                    "name": "Balanced U",
                    "type": "label"
                  }
                ],
                "id": "5af5c3c817584bbc736d5368",
                "ingredients": "Tomatoes Fresh Each Slice 1/4\"",
                "mrn": "47955",
                "mrn_full": "47955.4",
                "name": "Sliced Tomatoes",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061e18",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e19",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e1a",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e1b",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e1c",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e1d",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e1e",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e1f",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e20",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "1",
                    "value_numeric": "1"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e21",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e22",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e23",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "2 slice",
                "qty": null,
                "rev": "4",
                "sort_order": 20,
                "webtrition_id": 106457371
              },
              {
                "calories": 5,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fcf",
                    "name": "Onion",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  },
                  {
                    "id": "5a67f531a4227a2fac230c8e",
                    "name": "Balanced U",
                    "type": "label"
                  }
                ],
                "id": "5af4f39317584bbc736d5014",
                "ingredients": "Onions Red Fresh Each Slice",
                "mrn": "14918",
                "mrn_full": "14918.0",
                "name": "Red Onion Slice",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061e24",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "5",
                    "value_numeric": "5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e25",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e26",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e27",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e28",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e29",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e2a",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e2b",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e2c",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "1",
                    "value_numeric": "1"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e2d",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e2e",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e2f",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0",
                    "value_numeric": "0"
                  }
                ],
                "portion": "1 slice",
                "qty": null,
                "rev": "0",
                "sort_order": 21,
                "webtrition_id": 106457364
              },
              {
                "calories": 150,
                "custom_allergens": [],
                "desc": null,
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd3",
                    "name": "Vegan",
                    "type": "label"
                  },
                  {
                    "id": "5934c5733191a24f12b53002",
                    "name": "Soy",
                    "type": "allergen"
                  }
                ],
                "id": "5b2022f3efeb90a78e9212a5",
                "ingredients": "Potatoes Chips Skin-on Frozen, Salt Bulk, Spice Pepper Black Ground",
                "mrn": "103601",
                "mrn_full": "103601.0",
                "name": "House Fried Potato Chips ",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061e30",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "150",
                    "value_numeric": "150"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e31",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "110",
                    "value_numeric": "110"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e32",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e33",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e34",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "< 1",
                    "value_numeric": "<1"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e35",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "1.5",
                    "value_numeric": "1.5"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e36",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "280",
                    "value_numeric": "280"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e37",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e38",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "9",
                    "value_numeric": "9"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e39",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "12",
                    "value_numeric": "12"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e3a",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "0",
                    "value_numeric": "0"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e3b",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "0+",
                    "value_numeric": "0+"
                  }
                ],
                "portion": "1-1/2 ounce",
                "qty": null,
                "rev": "0",
                "sort_order": 22,
                "webtrition_id": 106457359
              },
              {
                "calories": 560,
                "custom_allergens": [],
                "desc": "Tunisian Harissa Aioli",
                "filters": [
                  {
                    "id": "5934c5723191a24f12b52fcf",
                    "name": "Onion",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd0",
                    "name": "Sulphites",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd1",
                    "name": "Tomato",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5723191a24f12b52fd2",
                    "name": "Vegetarian",
                    "type": "label"
                  },
                  {
                    "id": "5934c5733191a24f12b52fef",
                    "name": "Alcohol",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff1",
                    "name": "Egg",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5733191a24f12b52ff2",
                    "name": "Garlic",
                    "type": "allergen"
                  },
                  {
                    "id": "5934c5743191a24f12b53029",
                    "name": "Mustard",
                    "type": "allergen"
                  }
                ],
                "id": "5a65371628d0e73e15f92c65",
                "ingredients": "Oil Olive Extra Virgin, Onions Red Fresh Chopped Fine, Spice Chile Pepper Chipotle, Juice Lemon, Oil Canola, Tomato Paste Canned, Egg Fresh Separated Yolk Only, Garlic Cloves Peeled Fresh Crushed, Salt Kosher, Mustard Dijon, Spice Caraway Seed, Spice Cumin Seed, Spice Coriander Seeds",
                "mrn": "105833",
                "mrn_full": "105833.0",
                "name": "Harissa Aioli",
                "nutrients": [
                  {
                    "id": "5d23f95a4198d409c3061e3c",
                    "name": "Calories",
                    "uom": "kcal",
                    "value": "560",
                    "value_numeric": "560"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e3d",
                    "name": "Calories From Fat",
                    "uom": "kcal",
                    "value": "520",
                    "value_numeric": "520"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e3e",
                    "name": "Cholesterol (mg)",
                    "uom": "mg",
                    "value": "40",
                    "value_numeric": "40"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e3f",
                    "name": "Dietary Fiber (g)",
                    "uom": "g",
                    "value": "4",
                    "value_numeric": "4"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e40",
                    "name": "Protein (g)",
                    "uom": "g",
                    "value": "3",
                    "value_numeric": "3"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e41",
                    "name": "Saturated Fat (g)",
                    "uom": "g",
                    "value": "8",
                    "value_numeric": "8"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e42",
                    "name": "Sodium (mg)",
                    "uom": "mg",
                    "value": "440",
                    "value_numeric": "440"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e43",
                    "name": "Sugar (g)",
                    "uom": "g",
                    "value": "3+",
                    "value_numeric": "3+"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e44",
                    "name": "Total Carbohydrates (g)",
                    "uom": "g",
                    "value": "12",
                    "value_numeric": "12"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e45",
                    "name": "Total Fat (g)",
                    "uom": "g",
                    "value": "58",
                    "value_numeric": "58"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e46",
                    "name": "Trans Fat (g)",
                    "uom": "g",
                    "value": "-",
                    "value_numeric": "-"
                  },
                  {
                    "id": "5d23f95a4198d409c3061e47",
                    "name": "Vitamin D (IU)",
                    "uom": "IU",
                    "value": "10+",
                    "value_numeric": "10+"
                  }
                ],
                "portion": "1 tbsp",
                "qty": null,
                "rev": "0",
                "sort_order": 25,
                "webtrition_id": 106457358
              }
            ],
            "name": "Deli",
            "sort_order": 6
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

`GET http://kapi.dineoncampus.com/menu`

### Query Parameters

| Parameter   | Required | Description                                              |
| ----------- | -------- | -------------------------------------------------------- |
| site_id     | yes      | The Id of your site should be provided to you.           |
| location_id | yes      | The location Id. Obtained using the /locations endpoint. |
| platform    | yes      | Should be set to 0.                                      |
| date        | yes      | Formatted as YYYY-MM-DD                                  |

<aside class="success">
Remember — all requests are monitored. Please don't be spammy with your services 😀.
</aside>
