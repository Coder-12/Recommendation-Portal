# Recommendation-Portal
This API documentation serves as a reference to both backend and frontend members of recommendater portal. Few things to note that Schema here refers to the way the data will be stored in the database. Ideally, you can expect the same data to be returned to you in a JSON-compatible format. API routes refers to API specification of application.Each route has been designed to be as agnostic as possible. The API routes marked with (\*) are private routes and will have to be requested with user's JSON Web Token in the header. Following is the header that you must include along with your request to said API routes for access.<br/>
{<br/>
    "Authentication": "Bearer [token]" <br/>
}<br/>
Unless otherwise specified, the standard successful response to any request will be a JSON:<br/>
{<br/>
   "success": bool[true/false]<br/>
   "data": dict[Optional] (if some data is requested then only)<br/>
   "error": dict[Optional] (if success is false)<br/>
}<br/>
