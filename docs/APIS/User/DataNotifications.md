To allow you to create a dynamic website, the frontend version of our User API also allows you to listen some changes. For example, you can listen to leaderboards, to allow the users to view the latest scores without having to refresh the page.

For example, internally in the Awesome Bar, we listen to:
* The current user notifications, to display them in real time.
* The current user, to update the current balance of the user.

![](https://raw.githubusercontent.com/SuperAwesomeLTD/sa-club-documentation/develop/docs/img/notifications.png "API notifications example")

1. <span style="font-weight: 800;">The user visits a page or perform an action on a page</span>
2. <span style="font-weight: 800;">This will trigger a call to our API</span>
3. <span style="color: gray;">When an update is available, it will automatically be sent to you</span>
4. <span style="color: gray;">Our SDK will process it and send it to your listener</span>
5. <span style="font-weight: 800;">Your application will process it and update the page</span>