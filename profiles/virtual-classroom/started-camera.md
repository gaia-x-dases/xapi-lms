# Started camera

## Description

A user has started the camera. The action has been done by the participant itself or by another participant with moderation rights on the virtual classroom cameras. 

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
      "id": "http://schema.dases.eu/xapi/profile/virtual-classroom/verb/started-camera"
   },
   "object": {
      "objectType": "Agent",
      "account": {
         "name": "edward",
         "homePage": "http://gaiax-virtualclassroom.org"
      }
   },
   "context": {
      "extensions": {
         "http://schema.dases.eu/xapi/profile/virtual-classroom/extension/micro-activated": false
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
               "id": "http://schema.dases.eu/xapi/profile/virtual-classroom/templates/started-camera",
               "definition": {
                  "type": "http://adlnet.gov/expapi/activities/profile"
               }
            }
         ]
      }
   }
}
```