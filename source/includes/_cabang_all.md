# Cabang

## Get All Cabang

```shell
curl "http://localhost:PORT/cabang"
```

> The above command returns JSON structured like this:

```json
{
    "_links" : {
      "self" : {
        "href" : "http://localhost:8082/cabang{?page,size,sort}",
        "templated" : true
      },
      "next" : {
        "href" : "http://localhost:8082/cabang?page=1&size=20{&sort}",
        "templated" : true
      }
    },
    "_embedded" : {
      "cabang" : [ {
        "utype" : "KCP",
        "branchCode" : "0320",
        "name" : "Ambarawa",
        "address" : "Alamat Cabang Ambarawa",
        "city" : "Ambarawa",
        "latitude" : -7.256816,
        "longitude" : 110.40563,
        "_links" : {
          "self" : {
            "href" : "http://localhost:8082/cabang/1"
          }
        }
      }, {
        "utype" : "KCU",
        "branchCode" : "0044",
        "name" : "AMBON",
        "address" : "Alamat Cabang AMBON",
        "city" : "Ambon",
        "latitude" : -3.695889,
        "longitude" : 128.18217,
        "_links" : {
          "self" : {
            "href" : "http://localhost:8082/cabang/2"
          }
        }
      }, ]
    },
      "page" : {
      "size" : 20,
      "totalElements" : 237,
      "totalPages" : 12,
      "number" : 0
  }
}
```

This endpoint retrieves all Cabang.

### HTTP Request

`GET http://localhost:PORT/cabang`

