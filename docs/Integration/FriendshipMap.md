<span style="color: #ff0000;">Note: The following endpoint is only accessible from the application api as it contains information that the owner of the application might want to keep private. You’ll need to use the latest version:</span>

https://s3-eu-west-1.amazonaws.com/tmp-fix-github-ddos/sa-platform-node-sdk-a300741a0cdfe50391d84463b6434d88cf3131bc.tar.gz

```javascript
saAppApi.users.getUsersMap().then(function(response){
    // Do something
})
```

The results will be an objects mapping ISO 3166-2 to the number of users in that area:

```json
{
    'GB-CON': {name: "Cornwall", count: 91},
    'GB-COV': {name: "Coventry", count: 16},
    'GB-CRF': {name: "Cardiff", count: 42},
    'GB-CRY': {name: "Croydon", count: 62},
    // ...
}
```

<span style="color: #38761d;">Note: If you have some problems transforming these results into an image, please let us know and we will help you.</span>

<span style="color: #38761d;">Note: The endpoint is not yet fully implemented on our side so at the moment you’ll always receive the same result.</span>
