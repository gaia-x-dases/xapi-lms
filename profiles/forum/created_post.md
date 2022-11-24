# Created a post

## Description

The user has created a post within a topic.

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
      "id": "https://w3id.org/xapi/dod-isd/verbs/created"
   },
   "object": {
      "objectType": "Activity",
      "id": "http://gaiax.org/xapi/activities/20869a74-6c0d-11ed-a1eb-0242ac120002",
      "definition": {
         "type": "https://w3id.org/xapi/acrossx/activities/message",
         "name": {
            "en": "Test Post"
         }
      }
   },
   "context": {
      "contextActivities": {
         "parent": [
            {
               "id": "http://gaiax.org/xapi/activities/c5dd5f60-6c0a-11ed-a1eb-0242ac120002",
               "definition": {
                  "type": "http://id.tincanapi.com/activitytype/discussion"
               }
            }
         ],
         "grouping": [
            {
                "id": "http://gaiax.org/xapi/activities/706b5456-6c0a-11ed-a1eb-0242ac120002",
                "definition": {
                    "type": "http://id.tincanapi.com/activitytype/community-site"
                }
            }
         ]
      }
   }
}
```