# Posted private message (WIP)

## Description

A participant has sent a private message to another participant within the chat.

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
      "id": "http://adlnet.gov/expapi/verbs/posted"
   },
   "object": {
      "objectType": "Activity",
      "id": "http://gaiax.org/xapi/activities/f3757ec4-e427-4e3e-a934-fbccdd440a32",
      "definition": {
         "type": "https://w3id.org/xapi/acrossx/activities/message",
         "name": {
            "en": "Message of John #23"
         }
      }
   },
   "context": {
      "extensions": {
         "http://id.tincanapi.com/activitytype/chat-channel": "uuid://1a784f01-ec6a-4fa1-a95a-8c72280c4320"
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
               "id": "http://schema.dases.eu/xapi/profile/virtual-classroom/templates/posted-private-message",
               "definition": {
                  "type": "http://adlnet.gov/expapi/activities/profile"
               }
            }
         ]
      }
   }
}
```