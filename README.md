# REST vs GraphQL

## Comparison

<img src="attachments/387177950/387177257.png" width="600"/><br/>

|REST|GraphQL|
|-----|------|
|Defines structure of responses on the **server**|Defines structure of responses on the **client**|
|You might need multiple requests to get the actual data. This situation is referred to as **(n+1) problem**. |You can have all the fields and relationship defined and **fetched in a single request**.|
|For each new version of the response, or each variation of response data, you need a server developer to do coding.|You don't need a server developer to do coding if there is a change required for the response. Just, change the request and you will get what you want.|
|Strictly typed in nature (like SOAP's WSDL)|Not type enstricted|

## Verdict

It could be ideal if you use GraphQL as an abstraction and wraps over REST, so mobile clients could make a single request and fetch all the response needed in a single call. As well as, web clients could directly hit REST services as required.
