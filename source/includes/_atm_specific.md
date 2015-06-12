## Get a Specific ATM

```shell
curl "http://localhost:PORT/atm/1"

```

> The above command returns JSON structured like this:

```json
{
    "name" : "000A-Wisma Asia I",
    "address" : "ALAMAT ATM 000A-Wisma Asia I",
    "city" : "Jakarta Barat",
    "latitude" : -6.188951,
    "longitude" : 106.79753,
    "wsid" : "SAMPLE1",
    "_links" : {
      "self" : {
        "href" : "http://localhost:8082/atm/1"
      }
    }
}
```

This endpoint retrieves a specific ATM.

### HTTP Request

`GET http://localhost:PORT/atm/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the ATM to retrieve

