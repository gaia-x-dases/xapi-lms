# Left

## Description

A participant has left the virtual classroom session.

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
      "id": "http://activitystrea.ms/leave"
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
               "id": "http://schema.dases.eu/xapi/profile/virtual-classroom/templates/left",
               "definition": {
                  "type": "http://adlnet.gov/expapi/activities/profile"
               }
            }
         ]
      }
   }
}
```