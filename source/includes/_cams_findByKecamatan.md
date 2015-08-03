## Find CAMS in certain "kecamatan"

```shell
curl "http://localhost:PORT/cams/search/findByKecamatan?kecamatan=KELAPA GADING"

```

> The above command returns JSON structured like this:

```json
{
  "_embedded" : {
    "cams" : [ {
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
    }, {
      "namaDebitur" : "DEBITUR-2",
      "tglBap" : "24-Jan-2014",
      "alamatJaminan_1" : "Komp. Ruko Kirana Boutique Office",
      "kelurahan" : "KELAPA GADING TIMUR",
      "kecamatan" : "KELAPA GADING",
      "kodePos" : 14240.0,
      "latitude" : -6.167778,
      "longitude" : 106.884445,
      "_links" : {
        "self" : {
          "href" : "http://localhost:8082/cams/2"
        }
      }
    } ]
  }
}
```

This endpoint retrieves CAMS that resides in certain "kecamatan".

### HTTP Request

`GET http://localhost:PORT/cams/search/findBykecamatan?kecamatan=<NAME_OF_KECAMATAN>`

### URL Parameters

Parameter | Description
--------- | -----------
NAME_OF_KECAMATAN | The name of the "kecamatan"

