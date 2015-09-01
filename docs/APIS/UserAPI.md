The operation that you can perform include, for example:
* Points:
	* Get the balance of the current user
	* Get an history of the transactions
* Notifications:
	* Get the notifications of the user
	* “Read” notifications
* Games:
	* Get the rank of the user
	* Submit scores
* Painting competitions:
	* Submit entries


These operations can be performed from the frontend or from the backend of your application.

From the backend, the flow is the same as the Application API.

From the frontend:

![](https://raw.githubusercontent.com/SuperAwesomeLTD/sa-club-documentation/develop/docs/img/user-api-frontend.png "Application API usage flow (frontend)")

1. <b>The user will perform an action on your application</b>
2. <b>This will trigger a call to our API</b>
3. <span style="color: gray;">Our SDK will make a request to our API</span>
4. <span style="color: gray;">Our API will process the request and send a response</span>
5. <span style="color: gray;">Our SDK will process the response and send it to your application</span>
6. <b>Your application will process the response and update the page</b>