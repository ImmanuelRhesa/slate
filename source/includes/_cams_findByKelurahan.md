## Find CAMS in certain "kelurahan"

```shell
curl "http://localhost:PORT/cams/search/findByKelurahan?kelurahan=PEGANGSAAN DUA"

```

> The above command returns JSON structured like this:

```json
{
        "_embedded" : {
          "cams" : [ {
            "namaDebitur" : "DEBITUR-7",
            "tglBap" : "30-Jan-2014",
            "alamatJaminan_1" : "Jl. Ekspor I Blok H No.17,RT. 007 RW. 10",
            "kelurahan" : "PEGANGSAAN DUA",
            "kecamatan" : "KELAPA GADING",
            "kodePos" : 14250.0,
            "latitude" : -6.152,
            "longitude" : 106.9025,
            "_links" : {
              "self" : {
                "href" : "http://localhost:8082/cams/7"
              }
            }
          }, {
            "namaDebitur" : "DEBITUR-8",
            "tglBap" : "28-Jan-2014",
            "alamatJaminan_1" : "Perum. Kelapa Gading Pratama Jl. Griya",
            "kelurahan" : "PEGANGSAAN DUA",
            "kecamatan" : "KELAPA GADING",
            "kodePos" : 14250.0,
            "latitude" : -6.167778,
            "longitude" : 106.90222,
            "_links" : {
              "self" : {
                "href" : "http://localhost:8082/cams/8"
              }
            }
          } ]
        }
}
```

This endpoint retrieves CAMS that resides in certain "kelurahan".

### HTTP Request

`GET http://localhost:PORT/cams/search/findByKelurahan?kelurahan=<NAME_OF_KELURAHAN>`

### URL Parameters

Parameter | Description
--------- | -----------
NAME_OF_KELURAHAN | The name of the "kelurahan"

