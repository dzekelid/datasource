{
  "info": {
    "name": "Predix Analytics Runtime Healthcheck for custom datasource.",
    "_postman_id": "31ab68dd-129e-4a88-980e-729aec09fdf7",
    "description": "Indicates whether custom data connector is up and running.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Healthcheckcustom",
      "item": [
        {
          "id": "dd6845c4-3dd0-413a-ab13-18f891a801b4",
          "name": "healthcheck",
          "request": {
            "url": "{{default}}/api/v1/analytics/customdata/healthcheck",
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
            "description": "Indicates whether custom data connector is up and running."
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "da952b54-b5d0-460b-8f0c-244fccb420d7"
            }
          ]
        }
      ]
    }
  ],
  "variable": [
    {
      "key": "default",
      "value": "http://www.example.com/"
    }
  ]
}