## Edit ATM for insert Image Link

```shell
curl -H "Content-Type: application/json" -X PATCH -d "{\"image\": \"C:/xampp/htdocs/img/238\"}" http://localhost:8082/atm/238

```

> The above command returns JSON structured like this:

```json
{
  "name": "000A-Wisma Asia I",
  "address": "ALAMAT ATM 000A-Wisma Asia I",
  "city": "Jakarta Barat",
  "latitude": -6.188951,
  "longitude": 106.79753,
  "wsid": "SAMPLE1",
  "image": "C:/xampp/htdocs/img/238",
  "_links": {
    "self": {
      "href": "http://localhost:8082/atm/238"
    }
  }
}
```

This endpoint edit an ATM.

### HTTP Request

`PATCH http://localhost:PORT/atm/{id}`

### URL Path

Parameter | Description
--------- | -----------
ID | Id of ATM you want to edit

