# OAuth2.0-Go
1. Create an instance of oauth.Config with 
a. your project’s Client ID text, 
b. project’s Client Secret text, 
c. the predefined authorization URL and …
d. token URL, 
e. URL for the data scope you want access to,
f. and the callback URL that Google should return the code to
2. Direct the user to Google Authentication page using AuthCodeURL()
3. When Google returns the authorization code to your URL, save the code.
4. Exchange the code for a token using a oauth.Transport type
5. Use the Transport which has the token to get the user details.
