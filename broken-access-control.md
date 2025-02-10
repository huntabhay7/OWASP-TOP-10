# 🔗 Broken Access Control

Websites have pages that are protected from regular visitors. For example, only the site's admin user should be able to access a page to manage other users. If a website visitor can access protected pages they are not meant to see, then the access controls are broken.



<figure><img src=".gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>

Here we can see that id parameter that shows the current users id number as well as information regarding this

ip/note.php?note\_id=1

ip/note.php?note\_id=2

in there we can say that we are able to change ID from 1 to 2 , so we Pop-up to Other Account

<figure><img src=".gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

ip/note.php?note\_id=0 (Here we get a Flag of Try Hack Me)

## Authentication&#x20;

<mark style="background-color:blue;">Who the users are</mark>&#x20;

## Authorization&#x20;

<mark style="color:purple;">The Process of Mapping each user to a Particular set of priviledges so that we know when to allow or Deny access to specific sections of a website</mark>

## Insecure Direct Object Reference (IDOR)

<mark style="background-color:orange;">occurs when a section on a site allows users to get information by using ID as a parameters</mark>

## Cross Origin Resource Sharing (CORS)

Cross-origin resource sharing is a mechanism that allows restricted resources on a web page to be accessed from another domain outside the domain from which the first resource was served.

## FUZZING

<mark style="background-color:red;">Software testing technique in which unforeseem values are sent to a parameters to understand how it behaves under different circumstances</mark>&#x20;



we will copy session id of paricular login ,then we will run this command

<mark style="background-color:green;">gobuster -c  "session  "  dir  -b 400,404,302,500  --wordlist /usr/share/dirbuster/medium.txt   --url  https://hospital.local/patients/home</mark>

<figure><img src=".gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>

<img src=".gitbook/assets/file.excalidraw (1).svg" alt="" class="gitbook-drawing">

