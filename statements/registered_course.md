# Registered to a course

## Description

The actor is registered to a course.

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
   "timestamp": "2016-06-09T15:34:26.887Z"
}
```

## Properties

| Property | Presence | Value |
|---|---|---|
| object.definition.type | INCLUDED | Must be `http://adlnet.gov/expapi/activities/course` |
| verb.id | INCLUDED | Must be `https://w3id.org/xapi/tla/verbs/registered` |

## Rules

| Rules | PRESENCE | Remarks |
|---|---|---|
| timestamp | INCLUDED | - |
| context.extensions.http://schema.dases.eu/xapi/profile/common/extension/starting-date | RECOMMENDED | Can be specified when this date is known |
| context.extensions.http://schema.dases.eu/xapi/profile/common/extension/ending-date | RECOMMENDED | Can be specified when this date is known |
| context.extensions.http://schema.dases.eu/xapi/profile/common/extension/role | RECOMMENDED | - |
