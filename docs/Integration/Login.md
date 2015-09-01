![](https://raw.githubusercontent.com/SuperAwesomeLTD/sa-club-documentation/develop/docs/img/login-flow.png "User login flow")

<span style="font-weight: 800;">1. The user will click on the login button on your website</span>

![](https://raw.githubusercontent.com/SuperAwesomeLTD/sa-club-documentation/develop/docs/img/login-button.png "Login button")

<span style="font-weight: 800;">2. The click handler will call our frontend SDK</span>

```html
<button class="sa_sign_in" onclick="saUserApi.authentication.signIn()"></button>
```

![](https://raw.githubusercontent.com/SuperAwesomeLTD/sa-club-documentation/develop/docs/img/login-code.png "Frontend code example")

<span style="color: gray;">3. The user will be redirected to the SuperAwesome Club</span>
<span style="color: gray;">4. The user will arrive to our login/account creation page</span>

![](https://raw.githubusercontent.com/SuperAwesomeLTD/sa-club-documentation/develop/docs/img/club-login-page.png "Redirection Login Page Example")

<span style="color: gray;">5. The user will login or create an account</span>
<span style="color: gray;">6. The user will be redirected to your backend</span>
<span style="color: gray;">7. Our router will handle the request</span>
<span style="color: gray;">8. Our backend SDK will check with the club that the authentication is valid</span>
<span style="color: gray;">9. The club will send back the information needed to complete the process</span>
<span style="color: gray;">10. Our backend SDK will do an internal redirection to the page of your choice (by default, the homepage)</span>
<span style="font-weight: 800;">11. You will render that page</span>
<span style="font-weight: 800;">12. And show the user that he is authenticated</span>

```javascript
saUserApi.authentication.getUser().then(function(user){ 
    // Do something
})
```
