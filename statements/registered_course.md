# Registered to a course

## Description

A user is registered to a course, whether it is self-registration or cohort-registration (a course instructor has registered the user).

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
      "id": "https://w3id.org/xapi/tla/verbs/registered"
   },
   "object": {
      "id": "http://gaiax.org/xapi/activities/ba297687-b1aa-4477-9efd-a782c8fdb90a",
      "definition": {
         "type": "http://adlnet.gov/expapi/activities/course",
         "name": {
            "en": "Test Course"
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
         "https://w3id.org/xapi/lms/extensions/starting-date": "2016-09-01T09:00:00.000Z",
         "https://w3id.org/xapi/lms/extensions/ending-date": "2016-12-01T00:00:00.000Z",
         "https://w3id.org/xapi/lms/extensions/role": "learner" 
      }
   },
   "timestamp": "2016-06-09T15:34:26.887Z"
}
```

## Determining properties

| Property | Value |
|---|---|
| `$.verb.id` | MUST be `https://w3id.org/xapi/tla/verbs/registered` |
| `$.object.definition.type` | MUST be `http://adlnet.gov/expapi/activities/course` |

## Rules

- `$.context.contextActivities.category`: INCLUDED, MUST contain an activity with the `https://w3id.org/xapi/lms` id.
- `$.context.extensions['https://w3id.org/xapi/lms/extensions/starting-date']`: RECOMMENDED, ISO 8601 datetime, can be specified when the date is known.
- `$.context.extensions['https://w3id.org/xapi/lms/extensions/ending-date']`: RECOMMENDED, ISO 8601 datetime, can be specified when the date is known.
- `$.context.extensions['https://w3id.org/xapi/lms/extensions/role']`: RECOMMENDED, str, assigned role of the user defined on the platform for the given course. For example: `admin`, `teacher`, `staff`, `learner`.
- `$.timestamp`: INCLUDED.
