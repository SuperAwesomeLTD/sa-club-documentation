![](https://raw.githubusercontent.com/SuperAwesomeLTD/sa-club-documentation/develop/docs/img/login-flow.png "User login flow")

<p style="font-weight: 800;">1. The user will click on the login button on your website</p>

![](https://raw.githubusercontent.com/SuperAwesomeLTD/sa-club-documentation/develop/docs/img/login-button.png "Login button")

<p style="font-weight: 800;">2. The click handler will call our frontend SDK</p>

```html
<button class="sa_sign_in" onclick="saUserApi.authentication.signIn()"></button>
```

![](https://raw.githubusercontent.com/SuperAwesomeLTD/sa-club-documentation/develop/docs/img/login-code.png "Frontend code example")

<p style="color: gray;">3. The user will be redirected to the SuperAwesome Club</p>
<p style="color: gray;">4. The user will arrive to our login/account creation page</p>

![](https://raw.githubusercontent.com/SuperAwesomeLTD/sa-club-documentation/develop/docs/img/club-login-page.png "Redirection Login Page Example")

<p style="color: gray;">5. The user will login or create an account</p>
<p style="color: gray;">6. The user will be redirected to your backend</p>
<p style="color: gray;">7. Our router will handle the request</p>
<p style="color: gray;">8. Our backend SDK will check with the club that the authentication is valid</p>
<p style="color: gray;">9. The club will send back the information needed to complete the process</p>
<p style="color: gray;">10. Our backend SDK will do an internal redirection to the page of your choice (by default, the homepage)</p>
<p style="font-weight: 800;">11. You will render that page</p>
<p style="font-weight: 800;">12. And show the user that he is authenticated</p>

```javascript
saUserApi.authentication.getUser().then(function(user){ 
    // Do something
})
```
