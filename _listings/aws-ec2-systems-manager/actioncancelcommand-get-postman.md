{
  "info": {
    "name": "Amazon EC2 Systems Manager API Cancel Command",
    "_postman_id": "b2502d1d-ecb7-45ba-a6aa-ad138d32ee22",
    "description": "Attempts to cancel the command specified by the Command ID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "08f809ec-30fd-48ff-bd59-2fa33aaf8fdc",
          "name": "addTagsToResource",
          "request": {
            "url": "http://example.com/api/?Action=AddTagsToResource?ResourceId=ResourceId&ResourceType=ResourceType&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds or overwrites one or more tags for the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "21018140-1de9-447f-922e-567568f63753"
            }
          ]
        }
      ]
    },
    {
      "name": "Cancel",
      "item": [
        {
          "id": "e65cea67-95fc-4bf3-afe6-b6c1bbba1ab6",
          "name": "cancelCommand",
          "request": {
            "url": "http://example.com/api/?Action=CancelCommand?CommandId=CommandId&InstanceIds=InstanceIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attempts to cancel the command specified by the Command ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a49263e9-60e8-426a-a689-314372a6ec6a"
            }
          ]
        }
      ]
    }
  ]
}