To allow you to create a dynamic website, the frontend version of our User API also allows you to listen some changes. For example, you can listen to leaderboards, to allow the users to view the latest scores without having to refresh the page.

For example, internally in the Awesome Bar, we listen to:
* The current user notifications, to display them in real time.
* The current user, to update the current balance of the user.

![](https://raw.githubusercontent.com/SuperAwesomeLTD/sa-club-documentation/develop/docs/img/notifications.png "API notifications example")

1. The user visits a page or perform an action on a page
2. This will trigger a call to our API
3. When an update is available, it will automatically be sent to you
4. Our SDK will process it and send it to your listener
5. Your application will process it and update the page