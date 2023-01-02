# Unmuted

## Description

A user has been unmuted. The action has been done by the participant itself or by another participant with moderation rights on the virtual classroom microphones.

## Example

```json
{
   "actor": {
      "objectType": "Agent",
      "account": {
         "name": "john",
         "homePage": "http://gaiax-virtualclassroom.org"
      }
   },
   "verb": {
      "id": "http://schema.dases.eu/xapi/profile/virtual-classroom/verb/unmuted"
   },
   "object": {
      "objectType": "Agent",
      "account": {
         "name": "john",
         "homePage": "http://gaiax-virtualclassroom.org"
      }
   },
   "context": {
      "extensions": {
         "https://w3id.org/xapi/video/extensions/volume": 1,
         "http://schema.dases.eu/xapi/profile/virtual-classroom/extension/camera-activated": true
      },
      "contextActivities": {
         "parent": [
            {
               "id": "http://gaiax.org/xapi/activities/e59490e1-ddf2-4c43-bfdc-14e274abc106",
               "definition": {
                  "type": "http://id.tincanapi.com/activitytype/webinar",
                  "name": {
                     "en": "Demonstration webinar"
                  }
               }
            }
         ],
         "category": [
            {
               "id": "http://schema.dases.eu/xapi/profile/virtual-classroom/templates/unmuted",
               "definition": {
                  "type": "http://adlnet.gov/expapi/activities/profile"
               }
            }
         ]
      }
   }
}
```