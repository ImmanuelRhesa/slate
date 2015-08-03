# CAMS

## Get All CAMS

```shell
curl "http://localhost:PORT/cams"
```

> The above command returns JSON structured like this:

```json
{
    "_links" : {
      "self" : {
        "href" : "http://localhost:8082/cams{?page,size,sort}",
        "templated" : true
      },
      "next" : {
        "href" : "http://localhost:8082/cams?page=1&size=20{&sort}",
        "templated" : true
      }
    },
      "_embedded" : {
        "cams" : [ {
          "namaDebitur" : "DEBITUR-200",
          "tglBap" : "19-Mar-2014",
          "alamatJaminan_1" : "Perum. Taman Nyiur, Jl. Taman Nyiur VII",
          "kelurahan" : "SUNTER AGUNG",
          "kecamatan" : "TANJUNG PRIOK",
          "kodePos" : 14540.0,
          "latitude" : -6.136361,
          "longitude" : 106.869835,
          "_links" : {
            "self" : {
              "href" : "http://localhost:8082/cams/200"
            }
          }
        }, {
          "namaDebitur" : "DEBITUR-201",
          "tglBap" : "14-Apr-2014",
          "alamatJaminan_1" : "Jl. Agung Utara 8-B Blok A-32 No. 11",
          "kelurahan" : "SUNTER AGUNG",
          "kecamatan" : "TANJUNG PRIOK",
          "kodePos" : 14350.0,
          "latitude" : -6.133806,
          "longitude" : 106.86014,
          "_links" : {
            "self" : {
              "href" : "http://localhost:8082/cams/201"
            }
          }
        } ]
      },
      "page" : {
        "size" : 20,
        "totalElements" : 274,
        "totalPages" : 14,
        "number" : 0
      }
}
```

This endpoint retrieves all cams.

### HTTP Request

`GET http://localhost:PORT/cams`

