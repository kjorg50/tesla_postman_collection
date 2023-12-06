# tesla_postman_collection

Collection of Postman requests to various (unofficial) Tesla API endpoints

Based off of these two unofficial API docs
* https://www.teslaapi.io
* https://tesla-api.timdorr.com

## Usage
First, use the [tesla_auth](https://github.com/adriankumpf/tesla_auth) tool to securely generate access tokens on your machine. FYI, these have a TTL of 8 hours. **DO NOT SHARE OR PUT THESE IN ANY REPO!**

Second, set the `access_token` collection variable to the token generated by tesla_auth. This is used as a `Bearer` token in the `Authorization` header for requests made to the API.

Third, call the "List all vehicles" and get the `id` of the vehicle you want to look at in more detail. Put this in the `id` collection variable.
