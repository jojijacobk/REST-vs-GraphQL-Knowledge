# REST vs GraphQL

## Comparison

<img src="attachments/387177950/387177257.png" width="800"/><br/>

|REST|GraphQL|
|-----|------|
|REST APIs exposes multiple routes such as api/posts/, api/comments etc . Each of them has to be called separately to get the necessary data.| GraphQL exposes a single end point that let's client query whatever data as needed.|

|It is like <br/> - going to town for grocery shop and bring veggies home, <br/> - then go to same town bakery and bring snacks home, <br/> - and again go to same town textiles shop | it is like <br/> - make a shopping list, send a guy to buy all things together <br/> - there is no predefined shopping list because each day the list changes <br/> - so GraphQL is highly efficient|

|Defines structure of responses on the **server**|Defines structure of responses on the **client**|
|You might need multiple requests to get the actual data. This situation is referred to as **(n+1) problem**. |You can have all the fields and relationship defined and **fetched in a single request**.|
|For each new version of the response, or each variation of response data, you need a server developer to do coding.|You don't need a server developer to do coding if there is a change required for the response. Just, change the request and you will get what you want.|
|Strictly typed in nature (like SOAP's WSDL)|Not type enstricted|

## Verdict

It could be ideal if you use GraphQL as an abstraction and wraps over REST, so mobile clients could make a single request and fetch all the response needed in a single call. As well as, web clients could directly hit REST services as required.
