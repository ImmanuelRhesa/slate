## Get a Specific CAMS

```shell
curl "http://localhost:PORT/cams/1"

```

> The above command returns JSON structured like this:

```json
{
        "namaDebitur" : "DEBITUR-1",
        "tglBap" : "17-Jan-2014",
        "alamatJaminan_1" : "Apt Gading Mediterania Residences Blok",
        "kelurahan" : "KELAPA GADING BARAT",
        "kecamatan" : "KELAPA GADING",
        "kodePos" : 14240.0,
        "latitude" : -6.151992,
        "longitude" : 106.899414,
        "_links" : {
          "self" : {
            "href" : "http://localhost:8082/cams/1"
          }
        }
}
```

This endpoint retrieves a specific CAMS.

### HTTP Request

`GET http://localhost:PORT/cams/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the CAMS to retrieve

