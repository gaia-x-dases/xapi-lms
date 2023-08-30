# Downloaded an audio 

## Description

A user has downloaded a file of `audio` type from an LMS or an e-learning platform.

> NB: As this template is related to `audio` Activity, it is inspired from templates of [Audio Profile](https://profiles.adlnet.gov/profile/0925e2b8-0330-45d8-ab44-4abcaa5479f8).

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
         "type": "https://w3id.org/xapi/video/activity-type/audio",
         "name": {
            "en": "xAPI 101 Podcast"
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
         "https://w3id.org/xapi/video/extensions/length": 1543.65,
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
| `$.object.definition.type` | MUST be `https://w3id.org/xapi/video/activity-type/audio` |


## Rules

- `$.context.contextActivities.category`: INCLUDED, MUST contain an activity with the `https://w3id.org/xapi/lms` id.
- `$.context.extensions['https://w3id.org/xapi/video/extensions/length']`: RECOMMENDED, positive float with maximum 3 decimals, MUST contain the value of the actual length of the media in seconds.
- `$.context.extensions['https://w3id.org/xapi/cmi5/context/extensions/sessionid']`: RECOMMENDED, UUID, MUST contain the ID of the active session where the audio was downloaded.
- `$.timestamp`: INCLUDED.