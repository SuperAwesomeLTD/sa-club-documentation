The treasure hunt items are displayed through treasure hunt placements

![](https://raw.githubusercontent.com/SuperAwesomeLTD/sa-club-documentation/develop/docs/img/treasure-hunt.png "Treasure Hunt Example")

```javascript
saUserApi.treasureHunts.getPlacementElement({placementId: 999999})
	.then(function (element) {
		$(element).appendTo($('fooBar'));
	})
```

Most of the time, getPlacementElement won’t return anything. From time to time, it will return a DOM element containing the image. If the user clicks on the image, he will trigger an event, get a notification and be redirected the the page defined on the treasure hunt item.

[Image]

On this page, you can then show which items have been found / are still to find.

```javascript
saUserApi.events.hasTriggeredEvents({eventIds: [991, 992, 993, 994]})
	.then(function (result) {
		// ....
	})
```

[Image]
