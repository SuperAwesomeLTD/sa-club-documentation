[image]

1. The user will click on the login button on your website

[image]

2. The click handler will call our frontend SDK

```html
<button class="sa_sign_in" onclick="saUserApi.authentication.signIn()"></button>
```

 [image]

3. The user will be redirected to the SuperAwesome Club
4. The user will arrive to our login/account creation page

[image]

5. The user will login or create an account
6. The user will be redirected to your backend
7. Our router will handle the request
8. Our backend SDK will check with the club that the authentication is valid
9. The club will send back the information needed to complete the process
10. Our backend SDK will do an internal redirection to the page of your choice (by default, the homepage)
11. You will render that page
12. And show the user that he is authenticated

```javascript
saUserApi.authentication.getUser().then(function(user){ 
    // Do something
})
```
