## Get a Specific Cabang

```shell
curl "http://localhost:PORT/cabang/1"

```

> The above command returns JSON structured like this:

```json
{
    "utype" : "KCP",
    "branchCode" : "0320",
    "name" : "Ambarawa",
    "address" : "Alamat Cabang Ambarawa",
    "city" : "Ambarawa",
    "latitude" : -7.256816,
    "longitude" : 110.40563,
    "_links" : {
      "self" : {
        "href" : "http://localhost:8082/cabang/1"
      }
    }
}
```

This endpoint retrieves a specific cabang.

### HTTP Request

`GET http://localhost:PORT/cabang/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the cabang to retrieve

