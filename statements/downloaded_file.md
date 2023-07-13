# Downloaded a file

## Description

This event is emitted when a user has downloaded a file such as a pdf, doc, txt, ppt, xls, csv, etc.

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
      "id": "https://w3id.org/xapi/netc/verbs/downloaded"
   },
   "object": {
      "id": "http://gaiax.org/xapi/activities/ba297687-b1aa-4477-9efd-a782c8fdb90a",
      "definition": {
         "type": "http://activitystrea.ms/file",
         "name": {
            "en": "Test Course"
         },
         "extensions": {
            "https://w3id.org/xapi/acrossx/extensions/type": "application/pdf"
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
      }
   },
   "timestamp": "2016-06-09T15:34:26.887Z"
}
```

## Determining properties

| Property  | Value         |
|----------------|-----------------|
| verb.id | Must be `https://w3id.org/xapi/netc/verbs/downloaded` |
| object.definition.type | Must be `http://activitystrea.ms/file` |

## Rules

- `context.contextActivities.category`: INCLUDED, MUST contain an activity with the `https://w3id.org/xapi/lms` id.
- `timestamp`: INCLUDED.
