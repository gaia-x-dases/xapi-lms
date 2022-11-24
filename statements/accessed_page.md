# Accessed a page

## Description

The actor has accessed a page of a LMS or a website.

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
      "id": "https://w3id.org/xapi/netc/verbs/accessed"
   },
   "object": {
      "objectType": "Activity",
      "id": "http://gaiax.org/xapi/activities/ba297687-b1aa-4477-9efd-a782c8fdb90a",
      "definition": {
         "type": "https://w3id.org/xapi/acrossx/activities/webpage",
         "name": {
            "en": "Test Course"
         },
         "extensions": {
            "https://w3id.org/xapi/acrossx/extensions/type": "course"
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
         "grouping": [
            {
               "id": "http://gaiax.org/xapi/activities/ba297687-b1aa-224255-9efd-a782c8fdb90a",
               "definition": {
                  "type": "https://w3id.org/xapi/acrossx/activities/webpage",
                  "extensions": {
                     "https://w3id.org/xapi/acrossx/extensions/type": "course_list"
                  }
               }
            }
         ],
         "category": [
            {
               "id": "https://profiles.adlnet.gov/xapi/bf76a8cc-f46a-4065-aa7b-443df4efc2be/v/1",
               "definition": {
                  "type": "http://adlnet.gov/expapi/activities/profile"
               }
            }
         ]
      }
   }
}
```