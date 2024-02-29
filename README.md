# CVApp-Azure

## Create Resource Group
A container which holds necessary resources for Azure Solution. All objects created in Azure for a project should belong to a Resource Group. This helps group objects together for easy management.

## Create Computer Vision Resource
### Home -> Create Resource -> Computer Vision -> Create
Fill up the necessary details and click create.

## Retreive Necessary Information from Computer Vision Resource
Identify the URL and key needed to make API Calls and access the API console.
API Console: https://westus.dev.cognitive.microsoft.com/docs/services/computer-vision-v3-2/operations/56f91f2e778daf14a499f21b

## Execute API Callssend
From API Console, select the resource region and fill out the required information. At the end click on send

## Response
Here is a response of our sample API Call. It's a Json Structure.



csp-billing-usage: CognitiveServices.ComputerVision.Categories=1,CognitiveServices.ComputerVision.Landmarks=1,CognitiveServices.ComputerVision.Transaction=1
x-envoy-upstream-service-time: 831
apim-request-id: 5d83ad0a-77b6-4af7-9034-5f043c3e647f
Strict-Transport-Security: max-age=31536000; includeSubDomains; preload
x-content-type-options: nosniff
x-ms-region: East US
Date: Thu, 29 Feb 2024 15:03:39 GMT
Content-Length: 272
Content-Type: application/json; charset=utf-8

{
  "categories": [{
    "name": "building_",
    "score": 0.94921875,
    "detail": {
      "landmarks": [{
        "name": "Eiffel Tower",
        "confidence": 0.9999598264694214
      }]
    }
  }],
  "requestId": "5d83ad0a-77b6-4af7-9034-5f043c3e647f",
  "metadata": {
    "height": 1999,
    "width": 1200,
    "format": "Jpeg"
  },
  "modelVersion": "2021-05-01"
}



