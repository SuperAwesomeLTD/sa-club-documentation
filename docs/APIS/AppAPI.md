The operation that you can perform include, for example:

* Users:
	* List all the users of the application
	* Reading their data (i.e. the emails), if you are authorised to do so 
* Notifications:
	* List the notifications sent by your application
	* Notify the users
* Events: (the events are used to reward Awesome Points through transactions)
	* Create new events
* Transactions:
	* List all the transactions of your application (to find out when and how you awarded points to users)
* Treasure hunts:
	* List the treasure hunts running on your application
	* Set up a new treasure hunt
	* Create new treasure hunt placements (to control where the items will appear)
* Painting competitions:
	* Create new competitions
	* Approve/reject the entries
	* Download the entries

This will also allow you to perform more high level operations. For example:
* See how many points were awarded by your application
* Set which permissions your application will require

These operations can also be performed directly through our dashboard.

![](https://raw.githubusercontent.com/SuperAwesomeLTD/sa-club-documentation/develop/docs/img/user-api-backend.png "Application API usage flow")

If you need to call the Application API, the flow will be:
1. <span style="font-weight: 800;">The user will perform an action on your application</span>
2. <span style="font-weight: 800;">This will trigger an ajax request to your backend</span>
3. <span style="font-weight: 800;">Your backend will call a function of our SDK</span>
4. <span style="color: gray;">Our SDK will make a request to our API</span>
5. <span style="color: gray;">Our API will process the request and send a response</span>
6. <span style="color: gray;">Our SDK will process the response and send it to your application</span>
7. <span style="font-weight: 800;">Your application will process the response and send it back to the frontend</span>
8. <span style="font-weight: 800;">The fronted will process the response and update the page</span>

If you call the Application API via a script, only the steps 3-6 will apply.

If you use our dashboard, you will be the user and only 1 and 8 will apply.