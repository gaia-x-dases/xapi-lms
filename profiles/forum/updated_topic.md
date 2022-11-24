# Updated a topic

## Description

The user has updated a topic within a community site or a forum.

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
      "id": "https://w3id.org/xapi/dod-isd/verbs/updated"
   },
   "object": {
      "objectType": "Activity",
      "id": "http://gaiax.org/xapi/activities/c5dd5f60-6c0a-11ed-a1eb-0242ac120002",
      "definition": {
         "type": "http://id.tincanapi.com/activitytype/discussion",
         "name": {
            "en": "Test Topic"
         }
      }
   },
   "context": {
      "contextActivities": {
         "parent": [
            {
               "id": "http://gaiax.org/xapi/activities/706b5456-6c0a-11ed-a1eb-0242ac120002",
               "definition": {
                  "type": "http://id.tincanapi.com/activitytype/community-site"
               }
            }
         ],
         "grouping": [
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