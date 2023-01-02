# Created poll

## Description

A poll has been created in the virtual classroom in order to collect participants opinions about a given question.

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
      "id": "http://activitystrea.ms/create"
   },
   "object": {
      "objectType": "Activity",
      "id": "http://gaiax.org/xapi/activities/a0f9f133-1ef2-4c2d-8677-bc33085a2346",
      "definition": {
         "type": "http://activitystrea.ms/question",
         "name": {
            "en": "When was Europe created?"
         }
      }
   },
   "result": {
      "extensions": {
         "http://schema.dases.eu/xapi/profile/virtual-classroom/extension/response-type": "textbox"
      }
   },
   "context": {
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
               "id": "http://schema.dases.eu/xapi/profile/virtual-classroom/templates/created-poll",
               "definition": {
                  "type": "http://adlnet.gov/expapi/activities/profile"
               }
            }
         ]
      }
   }
}
```