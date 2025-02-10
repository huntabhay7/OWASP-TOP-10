---
cover: >-
  https://images.unsplash.com/photo-1497124401559-3e75ec2ed794?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxiYXRtYW58ZW58MHx8fHwxNzA5NzA1MDMxfDA&ixlib=rb-4.0.3&q=85
coverY: 0
---

# 🦄 Logging & Monitoring Failures







<mark style="color:red;">Logging</mark>

<mark style="background-color:red;">Storing events , Failures ,or suspicious activity in some form that we can call upon later</mark>



we will try Dictonary attack , we already know the username -that is tom --- we will bruteforce the password :&#x20;

<mark style="background-color:orange;">ffuf -w /usr/share/dirb/wordlists/common.txt -u https://hospital.local/patients/login  -X POST -H "Content-Type:  application/x-www-form-urlencoded"  -d "username=tom\&password=FUZZ"  -fc 200</mark>

<figure><img src=".gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

&#x20;&#x20;

<figure><img src=".gitbook/assets/image (5).png" alt=""><figcaption><p>we got a password</p></figcaption></figure>

<figure><img src=".gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

## Handlers

How are we going to store the log ?

What format is the log going to be in?

Are we going to rotate it?
