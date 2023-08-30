# Accessed a page

## Description

A user has accessed or navigated a page on a LMS or an e-learning platform.

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
         "category": [
            {
               "id": "https://w3id.org/xapi/lms",
               "definition": {
                  "type": "http://adlnet.gov/expapi/activities/profile"
               }
            }
         ]
      }
   }
}
```

## Determining properties

| Property | Value |
|---|---|
| `$.verb.id` | MUST be `https://w3id.org/xapi/netc/verbs/accessed` |
| `$.object.definition.type` | MUST be `https://w3id.org/xapi/acrossx/activities/webpage` |

## Rules

- `$.object.definition.extensions['https://w3id.org/xapi/acrossx/extensions/type']`: RECOMMENDED, MUST specify the type of the webpage. Can be any of the following value: `course`, `course_list` or `user_space`.
- `$.context.contextActivities.category`: INCLUDED, MUST contain an activity with the `https://w3id.org/xapi/lms` id.
- `$.timestamp`: INCLUDED.
