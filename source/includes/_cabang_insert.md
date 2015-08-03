## Insert new "Cabang"

```shell
curl -H "Content-Type: application/json" -X POST -d "{\"utype\": \"KCP\",\"branchCode\": \"7777\",\"name\": \"Kota Baru\",\"address\": \"Alamat Cabang Kota Baru\",\"city\": \"Kota Baru\",\"latitude\": -7.356816,\"longitude\": 110.40563 }" http://localhost:8082/cabang

```

> The above command returns JSON structured like this:

```json
{
      "utype": "KCP",
      "branchCode": "7777",
      "name": "Kota Baru",
      "address": "Alamat Cabang Kota Baru",
      "city": "Kota Baru",
      "latitude": -7.356816,
      "longitude": 110.40563,
      "_links": {
        "self": {
          "href": "http://localhost:8082/cabang/816"
        }
      }
}
```

This endpoint insert new "Cabang".

### HTTP Request

`POST http://localhost:PORT/cabang/`
