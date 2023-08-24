# Downloaded a file

## Description

This event is emitted when a user has downloaded a file EXCEPTED video, audio or document files. For these types of file, the corresponding statements templates should be used ([downloaded a video](./downloaded_video.md), [downloaded an audio](./downloaded_audio.md) or [downloaded a document](./downloaded_document.md))

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
| `$.verb.id` | MUST be `https://w3id.org/xapi/netc/verbs/downloaded` |
| `$.object.definition.type` | Must be `http://activitystrea.ms/file` |

## Rules

- `$.object.definition.extensions['https://w3id.org/xapi/acrossx/extensions/type']`: RECOMMENDED, MUST specify the type of the downloaded file. `video`, `document` and `audio` are EXCLUDED.
- `$.context.extensions['https://w3id.org/xapi/cmi5/context/extensions/sessionid']`: RECOMMENDED, UUID, MUST contain the ID of the active session where the file was downloaded.
- `$.context.contextActivities.category`: INCLUDED, MUST contain an activity with the `https://w3id.org/xapi/lms` id.
- `$.timestamp`: INCLUDED.