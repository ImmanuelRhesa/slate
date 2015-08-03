## Insert new CAMS

```shell
curl -H "Content-Type: application/json" -X POST -d "{ \"namaDebitur\": \"DEBITUR-77\",\"tglBap\": \"9-Jul-2015\",\"alamatJaminan_1\": \"Apt Gading Mediterania Residences Blok\",\"kelurahan\": \"KELAPA GADING BARAT\",\"kecamatan\": \"KELAPA GADING\",\"kodePos\": 14240,\"latitude\": -6.151992,\"longitude\": 106.899414 }" http://localhost:8082/cams

```

> The above command returns JSON structured like this:

```json
{
    "namaDebitur": "DEBITUR-77",
    "tglBap": "9-Jul-2015",
    "alamatJaminan_1": "Apt Gading Mediterania Residences Blok",
    "kelurahan": "KELAPA GADING BARAT",
    "kecamatan": "KELAPA GADING",
    "kodePos": 14240,
    "latitude": -6.151992,
    "longitude": 106.899414,
    "_links": {
      "self": {
        "href": "http://localhost:8082/cams/818"
      }
    }
}
```

This endpoint insert new CAMS

### HTTP Request

`POST http://localhost:PORT/cams/`
