# ATM

## Get All ATM

```shell
curl "http://localhost:PORT/atm"
```

> The above command returns JSON structured like this:

```json
{
    "_links" : {
      "self" : {
        "href" : "http://localhost:8082/atm{?page,size,sort}",
        "templated" : true
      },
      "next" : {
        "href" : "http://localhost:8082/atm?page=1&size=20{&sort}",
        "templated" : true
      }
    },
    "_embedded" : {
      "atm" : [ {
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
      } , {
        "name" : "000F-Menara Ancol",
        "address" : "ALAMAT ATM 000F-Menara Ancol",
        "city" : "Jakarta Utara",
        "latitude" : -6.123485,
        "longitude" : 106.85451,
        "wsid" : "SAMPLE6",
        "_links" : {
          "self" : {
            "href" : "http://localhost:8082/atm/6"
          }
        }
      } ]
    },
    "page" : {
      "size" : 20,
      "totalElements" : 300,
      "totalPages" : 15,
      "number" : 0
    }
}
```

This endpoint retrieves all ATM.

### HTTP Request

`GET http://localhost:PORT/atm`

