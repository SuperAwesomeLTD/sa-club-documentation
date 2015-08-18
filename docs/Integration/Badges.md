You don’t need to store badges / ranks. Instead, you can compute them dynamically when needed. Example: (from the backend. Remove the req. for the frontend)

```javascript
return Promise.all([
	req.saUserApi.games.getGameScores({gameIds: ['???', '???']}),
	req.saUserApi.events.hasTriggeredEvents({eventIds: [1, 2, 3]})
]).spread(function (scores, triggeredEvents) {
	
});
```