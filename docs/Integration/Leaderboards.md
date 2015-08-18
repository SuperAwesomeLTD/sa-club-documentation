You can get a snapshot of a leaderboard from the backend and the frontend of your application.

From the frontend, you can also listen for updates to award the leaderboards as soon as the scores are submitted.

```javascript
saUserApi.games.addGameLeaderBoardListener({gameId: '?????'}),
	function (leaderBoard) {
		// ....
	}
);
```