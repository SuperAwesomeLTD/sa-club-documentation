Error name          | Meaning in the app api | Meaning in the user api
------------------- | ---------------------- | ------------------------------
AuthenticationError | Wrong app api key      | The user is not authenticated
AuthorisationError  | You don’t have enough rights to perform the operation<br>For example, the requested feature is not enabled for your app | You don’t have enough rights to perform the operation<br> For example, your are trying to get points with an event to this app
ValidationError     | Incorrect parameters   | Incorrect parameters
Error               | Any other error        | Any other error