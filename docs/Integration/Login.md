![](https://raw.githubusercontent.com/SuperAwesomeLTD/sa-club-documentation/develop/docs/img/login-flow.png "User login flow")

1. <span style="font-weight: 800;">The user will click on the login button on your website</span>

![](https://raw.githubusercontent.com/SuperAwesomeLTD/sa-club-documentation/develop/docs/img/login-button.png "Login button")

2. <span style="font-weight: 800;">The click handler will call our frontend SDK</span>

```html
<button class="sa_sign_in" onclick="saUserApi.authentication.signIn()"></button>
```

![](https://raw.githubusercontent.com/SuperAwesomeLTD/sa-club-documentation/develop/docs/img/login-code.png "Frontend code example")

3. <span style="color: gray;">The user will be redirected to the SuperAwesome Club</span>
4. <span style="color: gray;">The user will arrive to our login/account creation page</span>

![](https://raw.githubusercontent.com/SuperAwesomeLTD/sa-club-documentation/develop/docs/img/club-login-page.png "Redirection Login Page Example")

5. <span style="color: gray;">The user will login or create an account</span>
6. <span style="color: gray;">The user will be redirected to your backend</span>
7. <span style="color: gray;">Our router will handle the request</span>
8. <span style="color: gray;">Our backend SDK will check with the club that the authentication is valid</span>
9. <span style="color: gray;">The club will send back the information needed to complete the process</span>
10. <span style="color: gray;">Our backend SDK will do an internal redirection to the page of your choice (by default, the homepage)</span>
11. <span style="font-weight: 800;">You will render that page</span>
12. <span style="font-weight: 800;">And show the user that he is authenticated</span>

```javascript
saUserApi.authentication.getUser().then(function(user){ 
    // Do something
})
```
