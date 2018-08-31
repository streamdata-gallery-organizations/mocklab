{
  "info": {
    "name": "MockLab Delete Mappings",
    "_postman_id": "5a84f03f-b0e6-4b76-826a-38d7fbdb17ba",
    "description": "Delete all stub mappings",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Mappings",
      "item": [
        {
          "id": "b2527c4e-4436-405e-924f-ab2fb7a49d55",
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
              "id": "0c036751-4654-47d6-9dd9-98a868c3c87d"
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