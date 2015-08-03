## Find "Cabang" in certain city

```shell
curl "http://localhost:PORT/cabang/search/findByCity?city=Ambon"

```

> The above command returns JSON structured like this:

```json
{
  "_embedded" : {
    "cabang" : [ {
      "utype" : "KCU",
      "branchCode" : "0044",
      "name" : "AMBON",
      "address" : "Alamat Cabang AMBON",
      "city" : "Ambon",
      "latitude" : -3.695889,
      "longitude" : 128.18217,
      "_links" : {
        "self" : {
          "href" : "http://localhost:8082/cabang/2"
        }
      }
    }, {
      "utype" : "KCP",
      "branchCode" : "0415",
      "name" : "Mardika",
      "address" : "Alamat Cabang Mardika",
      "city" : "Ambon",
      "latitude" : -3.6900175,
      "longitude" : 128.18364,
      "_links" : {
        "self" : {
          "href" : "http://localhost:8082/cabang/3"
        }
      }
    } ]
  }
}
```

This endpoint retrieves "Cabang" that resides in certain city.

### HTTP Request

`GET http://localhost:PORT/cabang/search/findByCity?city=<CITY_NAME>`

### URL Parameters

Parameter | Description
--------- | -----------
CITY_NAME | The name of the city

