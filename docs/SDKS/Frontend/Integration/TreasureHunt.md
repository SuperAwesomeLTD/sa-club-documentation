The treasure hunt items are displayed through treasure hunt placements

[Image]

```javascript
saUserApi.treasureHunts.getPlacementElement({placementId: 999999})
	.then(function (element) {
		// ....
		$(element).appendTo($('fooBar'));
	})
```

Most of the time, getPlacementElement won’t return anything. From time to time, it will return a DOM element containing the image. If the user clicks on the image, he will trigger an event, get a notification and be redirected the the page defined on the treasure hunt item.