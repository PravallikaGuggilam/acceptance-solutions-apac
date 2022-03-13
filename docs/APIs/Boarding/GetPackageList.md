# Get Package List

This API is used to get package list. Merchants needs to add session 
token received during login api call in the header of this API.


## Endpoint

GET `/Externalboarding/secure/packages`

## Payload Example

### Request Payload

```json

{
  "appType": "API",
  "mccCode": "5813",
  "merchantType": "SM",
  "acceptanceType": "POSMOB",
  "typeOfBusiness": "SOLPROR",
  "international": "No",
  "iciciMerchant": "No",
  "dcc": "Yes",
  "fundingCurrency": "NET_AUD",
  "boardingType": "NEWMID",
  "merchantGrade": "NA",
  "newFundingAc": ""


```
  
***Token should be sent as Authorization.***

### Minimum Requirements

The below table contains the mandatory fields required for a successful request. The full request schemas are available in our [API Explorer](../api/?type=get&path=/Externalboarding/secure/appstatus/{appUrn}).

### Request
| Variable | Type | Length |  Mandatory/Optional/Conditional  | Description/Values |
| -------- | :-------: | :--: | :------------: | ------------------ |
| `appType` | *Json Property* | 10 | M | Application Type |
| `mccCode` | *Json Property* | 4 | M | Mcc Code |
| `merchantType` | *Json Property* |  | M | merchant Type |
| `acceptanceType` | *Json Property* |  | M | Acceptance Type |
| `typeOfBusiness` | *Json Property* |  | M | Type Of Business |
| `international` | *Json Property* |  | M | International |
| `iciciMerchant` | *Json Property* |  | M | ICICI Merchant |
| `dcc` | *Json Property* |  | M | DCC |
| `fundingCurrency` | *Json Property* |  | M | Funding Currency |
| `boardingType` | *Json Property* |  | M | BoardingType |
| `merchantGrade` | *Json Property* |  | M | Merchant Grade| 


### Successful Response Payload

```json
[
{
"id": "15001",
"name": "Test Package AU 1_NEWMID",
"desc": "NAB Test Package",
"shrtName": null,
"level": null,
"image": null,
"cnrInd": null,
"acceptanceType": "POSMOB",
"isInternational": "No",
"isDCC": "Yes",
"msfTariff": "Tiered I/C",
"fundingCurrency": "NET_AUD",
"preferential": "N",
"otpEnabled": true,
"sbPackageDesc": null,
"sbInstrumentsDesc": null,
"sbVASDesc": null,
"sbTerminalTypeDesc": null,
"sbPricingDesc": null,
"attributes": [
{
"category": "Package VAS",
"displayName": null,
"attributeList": [
{
"name": "Charge Slip Type",
"value": "E",
"codeType": "Package VAS",
"applicableForFilter": true
},
{
"name": "FDConnect",
"value": "Y",
"codeType": "Package VAS",
"applicableForFilter": true
},
{
"name": "Project Call Type",
"value": "ISO",
"codeType": "Package VAS",
"applicableForFilter": false
},
{
"name": "MVV Indicator",
"value": "Y",
"codeType": "Package VAS",
"applicableForFilter": false
},
{
"name": "Email / SMS Invoicing",
"value": "Y",
"codeType": "Package VAS",
"applicableForFilter": true
}
]
},
{
"category": "Additional Peripherals",
"displayName": null,
"attributeList": [
{
"name": "Peripharal2",
"value": "Peripheral 2",
"codeType": "Additional Peripherals",
"applicableForFilter": false
},
{
"name": "Peripharal4",
"value": "Peripheral 4",
"codeType": "Additional Peripherals",
"applicableForFilter": false
},
{
"name": "Peripharal3",
"value": "Peripheral 3",
"codeType": "Additional Peripherals",
"applicableForFilter": false
},
{
"name": "Peripharal5",
"value": "Peripheral 5",
"codeType": "Additional Peripherals",
"applicableForFilter": false
},
{
"name": "Peripharal1",
"value": "Peripheral 1",
"codeType": "Additional Peripherals",
"applicableForFilter": false
}
]
},
{
"category": "Package Currency Acceptance",
"displayName": null,
"attributeList": [
{
"name": "DCC",
"value": "Y",
"codeType": "Package Currency Acceptance",
"applicableForFilter": false
},
{
"name": "DCC PARTNER",
"value": "openFxFuture",
"codeType": "Package Currency Acceptance",
"applicableForFilter": false
},
{
"name": "International",
"value": "N",
"codeType": "Package Currency Acceptance",
"applicableForFilter": false
}
]
},
{
"category": "Package Acceptance",
"displayName": null,
"attributeList": [
{
"name": "POSMOB",
"value": "Y",
"codeType": "Package Acceptance",
"applicableForFilter": false
}
]
},
{
"category": "Package Info",
"displayName": null,
"attributeList": [
{
"name": "KET MERCHANT TAGING",
"value": "Key Merchant Tagging",
"codeType": "Package Info",
"applicableForFilter": false
},
{
"name": "Package ID",
"value": "477",
"codeType": "Package Info",
"applicableForFilter": false
},
{
"name": "Package Level",
"value": "NEWMID",
"codeType": "Package Info",
"applicableForFilter": false
},
{
"name": "Package Name",
"value": "Test Package AU 1",
"codeType": "Package Info",
"applicableForFilter": false
},
{
"name": "Number of Terminals",
"value": "10",
"codeType": "Package Info",
"applicableForFilter": false
},
{
"name": "Package Description",
"value": "NAB Test Package",
"codeType": "Package Info",
"applicableForFilter": false
},
{
"name": "Preferrential?",
"value": "Y",
"codeType": "Package Info",
"applicableForFilter": false
}
]
},
{
"category": "Package Schemes",
"displayName": null,
"attributeList": [
{
"name": "Master",
"value": "Y",
"codeType": "Package Schemes",
"applicableForFilter": true
},
{
"name": "AMEX",
"value": "Y",
"codeType": "Package Schemes",
"applicableForFilter": false
},
{
"name": "DND",
"value": "Y",
"codeType": "Package Schemes",
"applicableForFilter": false
},
{
"name": "VISA",
"value": "Y",
"codeType": "Package Schemes",
"applicableForFilter": true
},
{
"name": "CUP",
"value": "Y",
"codeType": "Package Schemes",
"applicableForFilter": false
}
]
},
{
"category": "Package Tariffs",
"displayName": null,
"attributeList": [
{
"name": "MDR",
"value": "Visa@2%,MC@1%,CUP@2% & EFTPOS@1.5%",
"codeType": "Package Tariffs",
"applicableForFilter": false
},
{
"name": "MSF Tariff",
"value": "Tiered I/C",
"codeType": "Package Tariffs",
"applicableForFilter": true
}
]
},
{
"category": "Additional Terminal Info",
"displayName": null,
"attributeList": [
{
"name": "Terminal Instruction 2",
"value": "Terminal Instruction3",
"codeType": "Additional Terminal Info",
"applicableForFilter": false
}
]
},
{
"category": "Package Card Types",
"displayName": null,
"attributeList": [
{
"name": "DEBIT",
"value": "Y",
"codeType": "Package Card Types",
"applicableForFilter": false
},
{
"name": "PREPAID",
"value": "Y",
"codeType": "Package Card Types",
"applicableForFilter": false
},
{
"name": "CREDIT",
"value": "Y",
"codeType": "Package Card Types",
"applicableForFilter": false
},
{
"name": "OFFUS",
"value": "Y",
"codeType": "Package Card Types",
"applicableForFilter": false
}
]
}
]
}
]
```

### Error Response Payload

```json
{
  "status": {
    "statusCode": 401,
    "message": "Token not found"
  }
}
```

### Response
| Variable | Type | Length |  Mandatory/Optional/Conditional  | Description/Values |
| -------- | :-------: | :--: | :------------: | ------------------ |
| `id` | *string* | 20 | M | Identification Number |




Below table provides the list of application's error code and its description.

| ErrorCode |  Description/Values |
| --------  | ------------------ |
|`401` |Token not found|  
|`200` |Success|
|`300` |Request Failure|
|`500` |Internal Server Error|
|`404` |Not Found|
|`502` |Request Timed Out|