# Viewed a topic

## Description

The user has viewed a topic within a forum, community site.

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
      "id": "http://gaiax.org/xapi/activities/c5dd5f60-6c0a-11ed-a1eb-0242ac120002",
      "definition": {
         "type": "http://id.tincanapi.com/activitytype/discussion",
         "name": {
            "en": "Test Topic"
         },
         "extensions": {
            "https://w3id.org/xapi/acrossx/extensions/total-items": 3,
            "https://w3id.org/xapi/acrossx/extensions/total-pages": 1
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
      },
      "extensions": {
        "http://www.risc-inc.com/annotator/extensions/page": 1
      }
   }
}
```