| Method ||||
| ------ | - | - | - |
| saAppApi.notifications.notify(parameters) ||||
| **Parameters** ||||
| name | type | default | comment |
| targetUserIds | array of integers | [ ] | the ids of the users of your application that should receive the notification |
| **Response** ||||
| A promise that will:
* be resolved without data if the notification was sent successfully 
or 
* be rejected with an error ||||
