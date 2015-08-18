Node.js

To include our backend SDK, simply add the following dependency to your project:

```json
{
    “dependencies”{
        “superawesome”: “https://s3-eu-west-1.amazonaws.com/tmp-fix-github-ddos/sa-platform-node-sdk-7370c7401677685c0fd8338452083a64f6b5e3ce.tar.gz”
    }
}
```

To use it, require the module and instantiate the Application API with your api keys.

```javascript
var SuperAwesomeAppApi = require('superawesome');
var saAppApi = new SuperAwesomeAppApi({
    saAppId: ‘mlp-friendship-club’, 
    saAppApiKey: ‘z7IIRjPePAgP4i8M2fjYWoYPmWi2tVc3’,
    saPlatformUrl: ‘https://staging.superawesome.club’,
    loginRedirectUrl: ‘/go/there/after/login’,
    logoutRedirectUrl: ‘/go/there/after/logout’
});
```

Then, add our router to your express application:

```javascript
app.use(saAppApi.router);
```

This will:
* Add the urls needed to implement the authentication (see below).
* On every request, it will give you access to the User API by adding the req.saUserApi attribute to the request.

You can modify where the user will be redirected after the login/logout by modifying respectively loginRedirectUrl and logoutRedirectUrl.