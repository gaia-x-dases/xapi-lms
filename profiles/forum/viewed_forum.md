# Viewed a forum

## Description

The user has viewed a forum.

## Example

```json
{
   "actor": {
      "objectType": "Agent",
      "account": {
         "name": "john",
         "homePage": "http://gaiax.org"
      }
   },
   "verb": {
      "id": "http://id.tincanapi.com/verb/viewed"
   },
   "object": {
      "objectType": "Activity",
      "id": "http://gaiax.org/xapi/activities/706b5456-6c0a-11ed-a1eb-0242ac120002",
      "definition": {
         "type": "http://id.tincanapi.com/activitytype/community-site",
         "name": {
            "en": "Test Forum"
         }
      }
   },
   "context": {
      "contextActivities": {
         "parent": [
            {
               "id": "http://gaiax.org/xapi/activities/62f8d794-6c0a-11ed-a1eb-0242ac120002",
               "definition": {
                  "type": "http://adlnet.gov/expapi/activities/course"
               }
            }
         ]
      }
   }
}
```