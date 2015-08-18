Notifications can be sent only from the backend of your application.

```javascript
saUserApi.notifications.notify({
	description: 'This is a notification',
	targetUserIds: [userId]
});
```

A notification can be sent to multiple users at the same time.

To check if a user has performed an action, you can trigger a specific event and award 0 points to the user. For example, this can be used to check if a user has already watched a video.