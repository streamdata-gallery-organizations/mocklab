{
  "info": {
    "name": "MockLab Get Mappings",
    "_postman_id": "4f85203c-b647-4ae9-a2d4-2024b30246a9",
    "description": "Get all stub mappings",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Mappings",
      "item": [
        {
          "id": "3534656a-0710-403e-9dee-79031ae9dd24",
          "name": "getMappings",
          "request": {
            "url": "{{default}}/mappings?limit=%7B%7D&offset=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get all stub mappings"
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "05a5329f-a3e1-4adc-9077-499946936342"
            }
          ]
        },
        {
          "id": "d2a5573c-88c4-4256-9978-eef87aafd592",
          "name": "deleteMappings",
          "request": {
            "url": "{{default}}/mappings",
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Delete all stub mappings"
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "a8d0b61a-fbed-40ad-b683-5797aadca411"
            }
          ]
        }
      ]
    }
  ],
  "variable": [
    {
      "key": "default",
      "value": "http://www.example.com/__admin"
    }
  ]
}