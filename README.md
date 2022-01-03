# Orchestrating Web Services with BPEL

## Prerequisites

- Oracle JDeveloper 12c
- Oracle WebLogic 12c
- OSB Application: https://github.com/alexjcm/osb-application

## Installation

Clone this repository:

```
git clone https://github.com/alexjcm/soa-application.git
```

To open the application from JDeveloper click on the **File** > **Open** menu and open the `*.jws` file of the newly cloned repository.


## Deployment

From JDeveloper right click on the project and then click **Deploy**.

## Test

Enpoint: http://localhost:7101/soa-infra/resources/default/Project_SYNC/MainRestService/order

Method: POST

Request example:

```json
{
    "order":{
        "taxIdentificationNumber":"1234",
        "product":[
            {
                "productCode": "P123",
                "quantity": 5
            },
            {
                "productCode": "P456",
                "quantity": 20
            }
        ]
    }
}
```

Response example:

```json
{
    "order": {
        "id": 121
    }
}
```

## Sample requests for the rest of the web services in Postman

https://www.postman.com/alexjcm/workspace/worskspace-shared/request/4498063-dcc8c9d2-61e8-4eec-95d6-552788cf0ce8

