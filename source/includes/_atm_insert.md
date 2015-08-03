## Insert new ATM

```shell
curl -H "Content-Type: application/json" -X POST -d "{\"name\": \"000R-ATM Tester\",\"address\": \"ALAMAT ATM 000R-Tester\",\"city\": \"Jakarta Barat\",\"latitude\": -7.188951,\"longitude\": 106.79753,\"wsid\": \"SAMPLE11\"}" http://localhost:8082/atm

```

> The above command returns JSON structured like this:

```json
{
    
    "name": "000R-ATM Tester",
    "address": "ALAMAT ATM 000R-Tester",
    "city": "Jakarta Barat",
    "latitude": -7.188951,
    "longitude": 106.79753,
    "wsid": "SAMPLE11"
    "_links": {
      "self": {
        "href": "http://localhost:8082/atm/815"
      }
    }
}
```

This endpoint insert new ATM.

### HTTP Request

`POST http://localhost:PORT/atm/`
