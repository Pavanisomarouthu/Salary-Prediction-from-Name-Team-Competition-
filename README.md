

**1. Ping the API Endpoint**

```Request```
```
  GET /ping
  Content-Type: application/json
```
```Response```
```
  {
    "Payments API is alive"
  }
```
---

**2. POST request to add payment**

```Request```
```
   POST /payments
   Content-Type: application/json
```
| Parameter      | Type          | Description  |
| ------------- |:-------------:| -----:|
| orderId      | String      | Id of Order |
| userId | String      |   Id of User  |
| totalPrice      | float32      | Price of the order |
| cardDetails | Integer      |   CardNumber details |
| expDate | Integer      |   expDate  |
| contactPhone | Integer      |   Phone number  |
| securityCode | Integer      |   CVV details  |

```Response```

|Parameter	|Type	|Description  |
|----|----|----|
| PaymentId      | String      | Id of Payment autogenerated|
| orderId      | String      | Id of Order |
| userId | String      |   Id of User  |
| totalPrice      | float32      | Price of the order |
| cardDetails | String      |   CardNumber details |
| expDate | String      |   expDate  |
| securityCode | String      |   CVV details  |
| contactPhone | String      |   Phone number  |
| OrderStatus | bool      |   Status of Payment  |
| PaymentDate | String      |   Date when payment is processed |


**3. GET request to get a particular paymentid**

```Request```
```
  GET /payment/paymentid
  Content-Type: application/json
 ```
 ```Response```
 
|Parameter	|Type	|Description  |
|----|----|----|
| PaymentId      | String      | Id of Payment autogenerated|
| orderId      | String      | Id of Order |
| userId | String      |   Id of User  |
| totalPrice      | float32      | Price of the order |
| cardDetails | String      |   CardNumber details |
| expDate | String      |   expDate  |
| securityCode | String      |   CVV details  |
| contactPhone | String      |   Phone number  |
| OrderStatus | bool      |   Status of Payment  |
| PaymentDate | String      |   Date when payment is processed |


---
**4. GET request to get all payments**

```Request```
```
  GET /payments
  Content-Type: application/json
 ```
 ```Response```
 
|Parameter	|Type	|Description  |
|----|----|----|
| PaymentId      | String      | Id of Payment autogenerated|
| orderId      | String      | Id of Order |
| userId | String      |   Id of User  |
| totalPrice      | float32      | Price of the order |
| cardDetails | String      |   CardNumber details |
| expDate | String      |   expDate  |
| securityCode | String      |   CVV details  |
| contactPhone | String      |   Phone number  |
| OrderStatus | bool      |   Status of Payment  |
| PaymentDate | String      |   Date when payment is processed |


---

**5.Delete the payment**

```Request```
```
   DELETE /payment/paymentid
   Content-Type: application/json
```


|Parameter	|Type |	Description|
|-----|-----|------|
|messsage	|String| Payment deleted |


