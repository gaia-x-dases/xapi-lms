# Terminated

## Description

The virtual classroom session has terminated. The session ends when the last participant has left the classroom or when an administrator has ended the session.

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
      "id": "http://adlnet.gov/expapi/verbs/terminated"
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
   "result": {
      "extensions": {
         "http://id.tincanapi.com/extension/duration": 27.47
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
               "id": "http://schema.dases.eu/xapi/profile/virtual-classroom/templates/terminated",
               "definition": {
                  "type": "http://adlnet.gov/expapi/activities/profile"
               }
            }
         ]
      }
   }
}
```