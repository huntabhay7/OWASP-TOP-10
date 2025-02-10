# ☠️ XML External Entity

<figure><img src=".gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

An XML External Entity (XXE) attack is a vulnerability that abuses features of XML parsers/data. It often allows an attacker to interact with any backend or external systems that the application itself can access and can allow the attacker to read the file on that system. They can also cause Denial of Service (DoS) attack or could use XXE to perform Server-Side Request Forgery (SSRF) inducing the web application to make requests to other applications. XXE may even enable port scanning and lead to remote code execution.



## there are two types of XML Attacks  <mark style="background-color:purple;">1- In-band</mark> <mark style="background-color:orange;">2-Out-band</mark>

1. An in-band XXE attack is the one in which the attacker can receive an immediate response to the XXE payload.
2. out-of-band XXE attacks (also called blind XXE), there is no immediate response from the web application and attacker has to reflect the output of their XXE payload to some other file or their own server.

<figure><img src=".gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

## &#x20;Why we use XML?

1. XML is platform-independent and programming language independent, thus it can be used on any system and supports the technology change when that happens.
2. The data stored and transported using XML can be changed at any point in time without affecting the data presentation.
3. XML allows validation using DTD and Schema. This validation ensures that the XML document is free from any syntax error.
4. XML simplifies data sharing between various systems because of its platform-independent nature. XML data doesn’t require any conversion when transferred between different systems

&#x20;    &#x20;

## &#x20;<mark style="background-color:orange;">`<?xml version="1.0" encoding="UTF-8"?>`</mark>

&#x20;<mark style="color:blue;">Above the line is called XML prolog and it specifies the XML version and the encoding used in the XML document. This line is not compulsory to use but it is considered a</mark> <mark style="color:blue;"></mark><mark style="color:blue;">`good practice`</mark> <mark style="color:blue;"></mark><mark style="color:blue;">to put that line in all your XML documents.</mark>

&#x20;`<?xml version="1.0" encoding="UTF-8"?>`\
`<mail>`\
&#x20;  `<to>falcon</to>`\
&#x20;  `<from>feast</from>`\
&#x20;  `<subject>About XXE</subject>`\
&#x20;  `<text>Teach about XXE</text>`\
`</mail>`
---------

\
In the above example the <mark style="background-color:purple;">`<mail>`</mark> <mark style="background-color:purple;"></mark><mark style="background-color:purple;">is the ROOT</mark> element of that document and `<to>`, `<from>`, `<subject>`, `<text>` are the children elements. If the <mark style="background-color:purple;">XML document doesn't have any root element then it would be considered</mark><mark style="background-color:purple;">`wrong`</mark> <mark style="background-color:purple;"></mark><mark style="background-color:purple;">or</mark> <mark style="background-color:purple;"></mark><mark style="background-color:purple;">`invalid`</mark> <mark style="background-color:purple;"></mark><mark style="background-color:purple;">XM</mark>



## &#x20;what is DTD in XML.

&#x20;
