# SigningCloud_API_Postman

This is a Postman collection for SigningCloud API.

To use this script please update the following environment variables:
- apiKey
- apiSecret
- uploadFilePath


Update Pre-request and Post-response Script in each API
- signer details e.g. name, email, contact


----------------------------------------------------
# SigningCloud_API_Bruno

This is contain Bruno collection for SigningCloud API.

Bruno is a fast, git-friendly API client for testing REST, GraphQL, and gRPC APIs. Open source alternative to Postman with offline-first design and no cloud sync.
The way to use is similar, you can also import the environment and edit to suit your needs accordingly

Currenly only contain basic API call, thos with X- is not yet fully convert from Postman to Bruno. Feel free to convert and update here.

https://www.usebruno.com/downloads

Previously, we are using https://postman-echo.com/post in the preupload document to get the base64 value of the document and set it into the environment.
However, if you are in an offline environment, you are not able to send out this request. 

To get back the same result in offline, you can download the mock-echo.war and deploy it to the tomcat. This class was compiled with Java 8 so it should work in our Tomcat.
Edit the URL in the Preupload document offline request. then run it 1st before you are the upload document API. You should see the base64 value is set in your Bruno environment.

This mock-echo also can be used in Postman, just deploy and change the request URL accordingly
