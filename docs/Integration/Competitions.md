The competitions are displayed through game elements

```javascript
saUserApi.games.getGameElement({gameId: '55c47f46118da01291a814ac'})
    .then(function(game) {
        $('.competition’).append(game);
    });
```

The competition will be responsive. To resize the competition, simply resize its container (in this example .competition).
