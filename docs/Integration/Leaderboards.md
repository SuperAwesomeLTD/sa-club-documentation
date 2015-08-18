You can get a snapshot of a leaderboard from the backend and the frontend of your application.

From the frontend, you can also listen for updates to award the leaderboards as soon as the scores are submitted.

```javascript
saUserApi.games.addGameLeaderBoardListener({gameId: '?????'}),
	function (leaderBoard) {
		// ....
	}
);
```

From the backend, you can get the leaderboard of the application
```javascript
saUserApi.games.getApplicationScore({
    // Be careful, month index starts at 0 in javascript...
    start: new Date(2015, 6, 10),
    end: new Date(2015, 7, 11)
}).then(function(response){
    // Do something
})
```