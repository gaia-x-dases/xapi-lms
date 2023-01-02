# Joined

## Description

A participant has joined the virtual classroom session.

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
      "id": "http://activitystrea.ms/join"
   },
   "object": {
      "objectType": "Activity",
      "id": "http://gaiax.org/xapi/activities/e59490e1-ddf2-4c43-bfdc-14e274abc106",
      "definition": {
         "type": "http://id.tincanapi.com/activitytype/webinar",
         "name": {
            "en": "Demonstration webinar"
         }
      }
   },
   "context": {
      "extensions": {
         "https://w3id.org/xapi/video/extensions/user-agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.31 (KHTML, like Gecko) Chrome/26.0.1410.43 Safari/537.31",
         "http://schema.dases.eu/xapi/profile/virtual-classroom/extension/camera-activated": true,
         "http://schema.dases.eu/xapi/profile/virtual-classroom/extension/micro-activated": false
      },
      "contextActivities": {
         "parent": [
            {
               "id": "http://gaiax.org/xapi/activities/ba297687-b1aa-455757-9efd-a782c8fdb90a",
               "definition": {
                  "type": "https://w3id.org/xapi/acrossx/activities/webpage",
                  "extensions": {
                     "https://w3id.org/xapi/acrossx/extensions/type": "course"
                  }
               }
            }
         ],
         "category": [
            {
               "id": "http://schema.dases.eu/xapi/profile/virtual-classroom/templates/joined",
               "definition": {
                  "type": "http://adlnet.gov/expapi/activities/profile"
               }
            }
         ]
      }
   }
}
```