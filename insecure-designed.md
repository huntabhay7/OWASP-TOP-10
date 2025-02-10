# 🥅 Insecure Designed

&#x20;<mark style="background-color:red;">Threat Modeling</mark>

&#x20;The Process of identifying the actors or events that could represent risks to our platform

&#x20;

&#x20;

&#x20;

&#x20; Input validation that is too permissive

&#x20;Lack of encryption at rest

&#x20;Cookies that store sensitive information

&#x20;Business logic errors

&#x20;Relying on Security through obscurity as a control

&#x20;Randomness that can be predicted

&#x20;



&#x20;                                                                         &#x20;**&#x20;&#x20;**<mark style="background-color:red;">**Insecure Designed**</mark>

&#x20;                                                         Insecure regardless of how its implemented

&#x20;                                                                                <mark style="background-color:green;">**Secure Designed**</mark>

&#x20;                                                        Could be vulnerable due to poor implementation

&#x20;                                                                                    <mark style="background-color:purple;">**Block Ciphers**</mark>

&#x20;                                                 Algorithms that encrypts data in small called blocks

&#x20;                                                        <mark style="background-color:yellow;">**Advanced Encryption Standard (AES)**</mark>

&#x20;                                                   A Block cipher that uses symmetric keys for encryption

&#x20;                                                                        <mark style="background-color:purple;">**Electric Code Book (ECB)**</mark>

&#x20;                                               A block cipher mode of operation that works mostly by applying substitution

&#x20;                                                                          to generate the cipher test



## why insecure designed added to OWASP -10

A smart design process can help prevent many problems and vulnerabilities along the way. Inclusion of threat modeling, secure development cycles, and other security testing in the development process can and will dramatically improve the native security of an application

<mark style="color:green;">Insecure design has been added to the OWASP Top 10 list in 2021 because of how vital it is. Without a solid security foundation, most applications will suffer and require an endless stream of patches to keep them from being negligently insecure</mark>.

## What is Insecure Designed&#x20;

At its core, insecure design is the lack of security controls being integrated into the application throughout the development cycle. This can have wide ranging and deep-rooted security consequences as the application itself is not designed with security in mind



## THM

<figure><img src=".gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

## &#x20;Whats vulnerable&#x20;

At summary, ultimately, any application that stores or fetches data where there are no validations or integrity checks in place for the data queried or retained. A few examples of applications of this nature are:

\- E-Commerce Sites\
\- Forums\
\- API's\
\- Application Runtimes (Tomcat, Jenkins, Jboss, etc)

## &#x20;Who developed the Tomcat application?

### &#x20;<mark style="background-color:purple;">The Apache Software Foundation</mark>

## &#x20;What is the name of the base-2 formatting that data is sent across a network as?

### <mark style="background-color:blue;">Binary</mark>



## <mark style="color:orange;">De(Serialization)</mark>

\
&#xNAN;_&#x4C;earning is best done through analogies_\
A Tourist approaches you in the street asking for directions. They're looking for a local landmark and got lost. Unfortunately, English isn't their strong point and nor do you speak their dialect either. What do you do? You draw a map of the route to the landmark because pictures cross language barriers, they were able to find the landmark. Nice! You've just serialised some information, where the tourist then deserialised it to find the landmark.

## <mark style="background-color:blue;">What does this mean?</mark>

Say you have a password of "password123" from a program that needs to be stored in a database on another system. To travel across a network this string/output needs to be converted to binary. Of course, the password needs to be stored as "password123" and not its binary notation. Once this reaches the database, it is converted or deserialised back into "password123" so it can be stored.

<figure><img src=".gitbook/assets/image (33).png" alt=""><figcaption><p>Simply, insecure deserialization occurs when data from an untrusted party (I.e. a hacker) gets executed because there is no filtering or input validation; the system assumes that the data is trustworthy and will execute it no holds barred.</p></figcaption></figure>

<figure><img src=".gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

## &#x20;<mark style="background-color:red;">wc -c /etc/passwd</mark> (wc = word count   , -c = gives output in number)
