# Downloaded a document

## Description

This event is emitted when a user has downloaded a file of `document` type.

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
      "id": "http://id.tincanapi.com/verb/downloaded"
   },
   "object": {
      "id": "http://gaiax.org/xapi/activities/ba297687-b1aa-4477-9efd-a782c8fdb90a",
      "definition": {
         "type": "http://id.tincanapi.com/activitytype/document",
         "name": {
            "en": "xAPI 101 Introduction notes"
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
         "https://w3id.org/xapi/cmi5/context/extensions/sessionid": "53ff781a-3c52-11ee-be56-0242ac120002"
      }
   },
   "timestamp": "2016-06-09T15:34:26.887Z"
}
```

## Determining properties

| Property | Value |
|---|---|
| `$.verb.id` | MUST be `http://id.tincanapi.com/verb/downloaded` |
| `$.object.definition.type` | MUST be `http://id.tincanapi.com/activitytype/document` |

## Rules

- `$.context.contextActivities.category`: INCLUDED, MUST contain an activity with the `https://w3id.org/xapi/lms` id.
- `$.context.extensions['https://w3id.org/xapi/cmi5/context/extensions/sessionid']`: RECOMMENDED, UUID, MUST contain the ID of the active session where the document was downloaded.
- `$.timestamp`: INCLUDED.