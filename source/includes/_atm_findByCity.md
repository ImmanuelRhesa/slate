## Find ATM in certain city

```shell
curl "http://localhost:PORT/atm/search/findByCity?city=Cianjur"

```

> The above command returns JSON structured like this:

```json
{
  "_embedded" : {
    "atm" : [ {
      "name" : "011V-Cipanas",
      "address" : "ALAMAT ATM 011V-Cipanas",
      "city" : "Cianjur",
      "latitude" : -6.7363944,
      "longitude" : 107.04125,
      "wsid" : "SAMPLE287",
      "_links" : {
        "self" : {
          "href" : "http://localhost:8082/atm/287"
        }
      }
    }, {
      "name" : "010C-Ciranjang",
      "address" : "ALAMAT ATM 010C-Ciranjang",
      "city" : "Cianjur",
      "latitude" : -6.81174,
      "longitude" : 107.2495,
      "wsid" : "SAMPLE244",
      "_links" : {
        "self" : {
          "href" : "http://localhost:8082/atm/244"
        }
      }
    }, {
      "name" : "010M-Mangunsarkoro",
      "address" : "ALAMAT ATM 010M-Mangunsarkoro",
      "city" : "Cianjur",
      "latitude" : -6.820016,
      "longitude" : 107.14213,
      "wsid" : "SAMPLE253",
      "_links" : {
        "self" : {
          "href" : "http://localhost:8082/atm/253"
        }
      }
    } ]
  }
}
```

This endpoint retrieves ATM that resides in certain city.

### HTTP Request

`GET http://localhost:PORT/atm/search/findByCity?city=<CITY_NAME>`

### URL Parameters

Parameter | Description
--------- | -----------
CITY_NAME | The name of the city

