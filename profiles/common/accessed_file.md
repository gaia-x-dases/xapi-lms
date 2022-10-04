# Accessed a file

## Description

This event is emitted when a user has accessed a file such as a pdf, doc, txt, ppt, xls, csv, etc.

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
         "type": "http://activitystrea.ms/file",
         "name": {
            "en": "Test Course"
         },
         "extensions": {
            "https://w3id.org/xapi/acrossx/extensions/type": "application/pdf"
         }
      }
   }
}
```