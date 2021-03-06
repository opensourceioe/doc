---
weight: 11
title: APIs
---

# API List

## Read Device

```matlab
package main

import "github.com/bep/kittn/auth"

func main() {
	api := auth.Authorize("meowmeowmeow")

	_ = api.GetKittens()
}
```


```python
import kittn

api = kittn.authorize('meowmeowmeow')
api.kittens.get()
```

> The above command returns JSON structured like this:

```json
[
  {
    "id": 1,
    "name": "Fluffums",
    "breed": "calico",
    "fluffiness": 6,
    "cuteness": 7
  },
  {
    "id": 2,
    "name": "Max",
    "breed": "unknown",
    "fluffiness": 5,
    "cuteness": 10
  }
]
```

To read or get the signal value available at the device terminal.

### HTTP Request

`GET https://us-central1-smartapp-iot.cloudfunctions.net/api/read/<APIKey>/<DeviceID>/<DevicePIN>`

### Query Parameters

Parameter | Required | Description
--------- | ------- | -----------
`<APIKey>` | true | API Key generated by the user.
`<DeviceID>` | true | Device ID generated by application.
`<DevicePIN>`| true | Device PIN generated by application.

<aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside>

## Write to Device