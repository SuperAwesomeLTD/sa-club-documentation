The points are awarded through events.

Each event has a unique token that can be used to trigger the event for the current user.

```javascript
saUserApi.events.triggerEventWithToken({token: 'abcdefg', points: 5});
```

The maximum number of points that you can award is set on the event.

This can be done from the frontend and the backend.

When you need to allow the user to “redeem a code”, you can simply ask them for the code and then use it as the token of the event.