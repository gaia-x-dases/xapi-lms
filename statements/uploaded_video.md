# Uploaded a video

## Description

A user has uploaded a file of `video` type to an LMS or an e-learning platform.

> NB: As this template is related to `video` Activity, it is inspired from templates of [Video Profile](https://profiles.adlnet.gov/profile/90b2c849-d744-4d0c-8bd0-403e7859a35b).

## Example

```json
{
   "actor": {
      "account": {
         "name": "john",
         "homePage": "http://gaiax.org"
      }
   },
   "verb": {
      "id": "https://w3id.org/xapi/netc/verbs/uploaded"
   },
   "object": {
      "id": "http://gaiax.org/xapi/activities/ba297687-b1aa-4477-9efd-a782c8fdb90a",
      "definition": {
         "type": "https://w3id.org/xapi/video/activity-type/video",
         "name": {
            "en": "xAPI 101 Introduction"
         }
      }
   },
   "context": {
      "contextActivities": {
         "category": [
            {
               "id": "https://w3id.org/xapi/lms",
               "definition": {
                  "type": "http://adlnet.gov/expapi/activities/profile"
               }
            }
         ]
      }, 
      "extensions": {
         "https://w3id.org/xapi/video/extensions/session-id": "53ff781a-3c52-11ee-be56-0242ac120002"
      }
   },
   "timestamp": "2016-06-09T15:34:26.887Z"
}
```

## Determining properties

| Property | Value |
|---|---|
| `$.verb.id` | MUST be `https://w3id.org/xapi/netc/verbs/uploaded` |
| `$.object.definition.type` | MUST be `https://w3id.org/xapi/video/activity-type/video` |

## Rules

- `$.context.contextActivities.category`: INCLUDED, MUST contain an activity with the `https://w3id.org/xapi/lms` id.
- `$.context.extensions['https://w3id.org/xapi/video/extensions/session-id']`: RECOMMENDED, UUID, MUST contain the ID of the active session where the video was downloaded.
- `$.timestamp`: INCLUDED.