# Week 2

### Grading

Task #|Points|Description|
-----|:---:|----------|
Task 1 | 1 | Browsers and Banking Security ***or*** Certifcates
Task 2 | 1 | Cards and Payments
Task 3 | 1 | Card Fraud
Task 4 | 1 | Non-technical Alternative 
Task 4 | 2 | Subdomain Takeover 

---

# Tasks

### Task 1: Choose A ***or*** B

#### Task 1A: Browsers and Banking Security

Online Banking is of the most lucrative targets for phishing and scams. How do our browsers protect us against them?

Look at the following snippets from a browsers address bar:

![Bank image 1](https://github.com/ouspg/SecurityEngineering/blob/main/Week2_Banking_and_Payments/Images/bank_1.png)

![Bank image 2](https://github.com/ouspg/SecurityEngineering/blob/main/Week2_Banking_and_Payments/Images/bank_2.png)

![Bank image 3](https://github.com/ouspg/SecurityEngineering/blob/main/Week2_Banking_and_Payments/Images/bank_3.png)

**Questions:**

- What does the "Not Secure" warning mean in the first picture and what risks does visiting sites with the warning pose?
    It means that between the exchange of packages between a user and a bank, the data is easily read by another user or a third-party.
- Why does the second site show up as "trusted" to the browser?
    Firstly, because different than the first one, this is a real domain, even using .io that is known to be not trustworthy but with a secure provider.
- What other ways are there to detect a phishing/scam site? 
    Paying attention to spams like pop-ups or written with words misspelled. Usually sites that ask for a bunch of clicks or have malicious links.  
    - Are there any tools available online?
    Searching for it online, i found a app called Kaspersky that blocks sites with malicious intentions behind it.
- What is typosquatting and how does it relate to the pictures?
    A form of cybersquatting, basically a site that uses a brand name as its domain. The first image shown is a misspelled domain or pretty similar to the original website.
    - What is **UDRP** and how does it help with combatting typosquatting?
    Administrative proceeding that complements or replaces court litigation over trademarks in domain names. Its helpful as it copyright claims similar domains to a main company one.
    - If you were to own the domain **ouspg.org** and would be running your crypto banking application at **bank.ouspg.org**, what domains could you monitor for warning signs of possible phishing attempts against your customers?
    It is better to choose the domain with more than one domain to protect and strengthen your business from competitive activity. 

#### Task 1B: Certificates

You have probably seen the following kind of warning when browsing the internet:

![Certificate image 1](https://github.com/ouspg/SecurityEngineering/blob/main/Week2_Banking_and_Payments/Images/certificate_1.png)

**Questions:**

- What are digital certificates used for?
Digital certificates serve several crucial purposes in the realm of online security, authentication, data encryption, integrity, non-repudiation. 
    - Why are certificates important for online payments and banking security?
    Certificates are vital for online payments and banking because they establish trust between the user's browser and the bank's website. When you access your bank's website, the bank presents its digital certificate to prove its identity.
    - What other uses do certificates have?
    Email security, VPN authentication
- What kind of attacks does TLS mitigate and why is this important for online banking?
    Eavesdropping, MITM, Data tempering, Phishing. In this context, TLS is important for banks because they safeguard confidentialy and integrity between finacial transactions and sensitive information from the customer as well.

- How do browsers use certificates for ensuring browsing security?
    By having a certificate on a webpage, it makes it possible to define the authenticity of the system by comparing with diferent authentic certificates, and it checks if the certificate was revoked and display a message depending of how is it.

    - What does the warning in the picture above mean?
        It warns about untrusted websites, that may have a third-party trying to steal information in the site.

**Certificate Authorities**

Read the following entries on Certificate Authorities and Certificate Transparency and answer questions:

https://en.wikipedia.org/wiki/Certificate_authority
https://en.wikipedia.org/wiki/Certificate_Transparency
https://certificate.transparency.dev/howctworks/
https://www.ecb.europa.eu/pub/pubbydate/html/index.en.html

**Questions:**

- Why would it be bad if a trusted certificate authority was compromised?
    If a trusted Certificate Authority (CA) were compromised, it would have significant and far-reaching consequences for internet security. Here are some reasons why it would be bad:
    Trust Erosion, Phishing and Man-in-the-Middle Attacks, Data Interception, Widespread Impact, Loss of Confidence

- Why is certificate transparency important?
    Certificate Transparency is important because it helps detect and prevent fraudulent certificate issuances, enhances the overall security of the internet, and ensures that CAs are held accountable for their role in securing online communications. It adds an additional layer of security and transparency to the SSL/TLS certificate issuance process, reducing the risk of misuse and abuse.
---

### Task 2: Cards and Payments

**Read the following:**

https://en.wikipedia.org/wiki/Payment_card
https://en.wikipedia.org/wiki/EMV
https://en.wikipedia.org/wiki/Multi-factor_authentication

**Questions: Payments**

- Why do modern payment cards use a chip and not a magnetic stripe?
    Chips are more secure than magnetic stripes because they don't transmit the card's real number during a transaction.
- What are EMV Certificates and why are they relevant for payment protection?
    Is a security protocol that reduces the chances of card fraud by encrypting the data on the chip. They are relevant because they are designed to ensure that point-of-sale devices, payment processors and acquiring banks comply to a standard.
- What attacks exist against payment cards?
    - Card-not-present?
    Stolen card details, phising, carding, account takeover
    - Contactless payment?
    Dataskimming, transaction relay attacks, counterfeit cards, lost and stolen cards

**Questions: MFA**

- How is multi-factor authentication (MFA) used in banking?
    A good example of a multi-factor authentication used in banking is ATM, you need to factors to access your account, the card and the security pin or password.
- How does multi-factor authentication increase payment security?
    Validates the authenticity of the person who carries the card, if it really is the owner the person would have no problem with the second authentication factor, the password.
- What MFA methods are you using in you daily life?
    Credit cards, i would say accounts in general because of having knowledge of account name or emails and passwords.
- What attacks exists against different forms of 2FA?
    - Time-based-one-time-password?
    Phishing, MITM(man in the middle), credential stuffing.
    - Text Message?
    SIM swapping, social engineering, phishing, Malware

---

### Task 3: Card Fraud

One part of understanding payment card security is monitoring how the cards are used for frauds. The following articles are reports on card fraud by the European Central Bank and will give you an overview of how the fraud landscape has evolved between 2008-2019. Read through the articles and then answer the questions in the questions section.

**Read the following reports:**


https://www.ecb.europa.eu/pub/pdf/cardfraud/cardfraudreport201207en.pdf
https://www.ecb.europa.eu/pub/cardfraud/html/ecb.cardfraudreport202008~521edb602b.en.html
https://www.ecb.europa.eu/pub/cardfraud/html/ecb.cardfraudreport202110~cac4c418e8.en.html

**Supporting Resources:**

https://www.ecb.europa.eu/pub/pubbydate/html/index.en.html (Search: "Fraud")
https://www.ecb.europa.eu/paym/intro/mip-online/2018/html/1803_revisedpsd.en.html


**Questions:**

    Write a summary (max 800 words) on "Evolution of card fraud" in which you answer at least the following questions:

    - What kinds of card fraud exist?
        - How does card fraud type prevalence differ geographically?
    - How has the fraud landscape changed between 2008-2019? Why?
        - What type of fraud has seen a notable increase during the last decade?
        - What technologies or regulations have had an impact on card fraud?
    - How has the transaction landscape changed in the same period?
        - What kind of transactions have become increasingly popular?
        - What kind of transactions have had a high risk of being fraudulent?
            - Has this changed at all during 2008-2019?
    - What effect has internet and e-commerce had on card fraud?
    - Why is preventing data breaches important in preventing card fraud?
        - How does payment card tokenisation help in this?
    -Anything interesting you found?

---
Card frauds has being into a continuity change into our modern world, that's because of factors such as technological advancements and regulations disposed into our society, card fraud are presented in several distinct categories, including Card-Not-Present (CNP) Fraud, Card-Present (CP) Fraud, Account Takeover (ATO), and Card Application Fraud. Each type has its unique characteristics and methods employed by fraudsters. A good example of geographic variation is Finland and Brazil, I'm from Brazil so the need of security is obvious and well known, that's because those variations depend on economical matters as well, for a third-world country to have its security compared to a first-world country is pragmatic. Between 2008-2019, we have had the rise of e-commerce and online baking leading to a increase on CNP frauds, the adoption of EMV chip cards, Increase of mobile payments. 
Account Takeover (ATO) fraud saw a significant increase in the last decade. Criminals exploited the availability of personal information online to impersonate individuals and gain unauthorized access to their accounts. Technological advancements like EMV chip cards and regulatory measures such as the Payment Card Industry Data Security Standard (PCI DSS) played significant roles in reducing fraud. EMV chip cards made card cloning more difficult, while PCI DSS imposed stringent security standards on organizations handling cardholder data.
Finally, it is trivial to know that one of the most impactful changes is the transaction landscape, with the development of new and advanced technology the world changed its ways of having transaction, with more ease and outgoing manners of realizing them but with that comes breaches in security 



## Task 4: Subdomain Takeover ***or*** Non-Technical Alternative

### Task 4: Subdomain Takeover

Practising use of browser developer tools and Python by playing out an example scenario of subdomain takeover on a simple Banking application.

## Pretask

Summarize in a few sentences what is a subdomain takeover?

- https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/02-Configuration_and_Deployment_Management_Testing/10-Test_for_Subdomain_Takeover
- https://developer.mozilla.org/en-US/docs/Web/Security/Subdomain_takeovers

```
Subdomain takeover is when a attacker gain control over a subdomain of a target domain.

```

## Requirements

This task requires `docker`.

## Summary

You have been tasked to test a new banking application developed by an intern at OUSPG which is riddled with bugs and flaws
in software design. In this exercise we will mainly look over the most obvious flaws in the application and focus on
subdomain takeover.

During development the application was created with a microservice architecture in mind and was originally deployed to
an application platform hosted by a hosting provider. However, later in development the service was moved to run on its
own servers and most of the microservice components were retired.

In this task you will get to familiarize yourself on how a subdomain takeover could happen and what effects it could
have. You will get to inspect a very simple web application and figure out how it works. You will also need to write
your own simple web server to receive data.

Completing this exercise will help you familiarize yourself with your browsers developer tools and Python programming.

## Task

To get started run `docker compose up` and follow the next few steps:

1. Open your browser to http://bank.ouspg.org.localhost:8080/
    - You should now see a screen with option `login` and `register`
    - Register a user to the site (for example `a` and `a`)
2. You should now be in the home screen again with a view of your balance and an option to send money.
3. Now logout from the application.

As this is all running locally, the subdomain takeover is not done by inspecting DNS, but rather analyzing faults within
the website itself.

#### Subdomain Takeover

Open up the [home page](http://bank.ouspg.org.localhost:8080/) again and the developer tools of your browser
(alt + f12).

__Task 1:__ Find out what the application does when you log in

- What methods get called and where?
    Methods that can be read are basically when logged the analyticsData add a counter, and sendData that are all blocked by chrome or a CORS response are ensuring validity.. 
    - _See the network tab of your browser's developer tools as well as the console_
- What data gets saved?
    User name, quantity of users online and the changeable balance
    - _See the storage tab of your browser's developer tools_
- Is any data sent to external services?
    The only user data that i could find that was sent is the amount of users online if a user is logged into the system, actually now i found that user information are sent to TODO: Send customer info to all subservices.
    URL Da Solicitação:
http://analytics.bank.ouspg.org.localhost:8080/
Método De Solicitação:
GET
Código De Status:
200 OK
Endereço Remoto:
127.0.0.1:8080
Política Do Referenciador:
strict-origin-when-cross-origin
    - _You can inspect the request headers and body via developer tools_
- Is there anything hazardous about the login process?
    Its been blocked by google chrome RSS, Mail, BSS, Quest, feed and check. 
```


```

__Task 2:__ Figure out which subdomain of the application is vulnerable to takeover

- How did you figure out the domain?
- How can you find out the hosting provider after finding out the domain?

```



```

<details>
    <summary>Hints</summary>

Try and see if any response in the network tab differs from the others.
Then try and navigate to that address while keeping an eye on your developer tools.
Inspect any responses you receive while investigating the domains.

</details>

__Task 3:__ Taking over the domain

Now that you found the target domain and the hosting provider, make an assumption that the subdomain was running in the
app engine of the provider. We will be simulating a small cloud provider which handles their ipv4 allocation by simply
provisioning them via roundrobin for any servers joining their app platform.

- Visit the imaginary cloud provider management portal at http://hosting-provider.org.localhost:8080/servers/docs
- Try out the functionality of the API portal and try to get the IP of the target subdomain under your control
    - You can see this by monitoring the target subdomain for a change in response

In this case the IP range is very small, and you can perform this task manually. However, in any real scenario the pool
of ip addresses would be big enough to warrant automation. Create a script to automatically provision servers until you
get the desired domain by utilizing the underlying API of the management portal:

```


```

<details>
    <summary>Hints</summary>

You can look at the _Network_ tab of you browsers developer tools while using the management page.
See any requests and their content when you click buttons on the page.
You can also use the inspect feature on most browsers and look into the page source.

For the script, you can use the `requests` library in python:

```python
import requests as r

r.post('http://my-server/my-path', json={
    'data': 'value'
})
```

</details>

__Task 4:__ Hijacking data

Your task is to create an application that collects users that log in to the application and hijacks their session if
they navigate to your subdomain page.

If you have trouble receiving the login callback data from the banking application, familiarize yourself with
[CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS) and make required adjustments.

Test your application by creating another user in the banking application and by navigating to your site.
You should be able to transfer all their money to your account.
You should also be able to receive callbacks from the banking application when users log in.

Place your code in the [create_your_server.py](create_your_server.py) file.

<details>
    <summary>Hints</summary>

Try and inspect the banking application and see what data it sends during login.
Also, inspect what data you possibly want to get from users when they land on your page.

You can take inspiration from [analytics.py](analytics.py)

You can use the provided script and add endpoints as follows:

```python
from fastapi import FastAPI, Request, Response, Cookie
from pydantic import BaseModel

app = FastAPI()


class MyAPIModel(BaseModel):
    value: str


@app.options('/')
def my_function(request: Request, response: Response):
    ...


@app.get('/')
def my_function(cookie_value: Cookie(alias='my-cookie')):
    return {
        'my-data': 'is-json'
    }


@app.post('/')
def my_function(model: MyAPIModel):
    ...

```

You can see the intro for [FastAPI](https://fastapi.tiangolo.com/tutorial/) for more guidance.

</details>

To finish off run `docker compose down -v` to delete any residual volumes.

__Task 5:__ Questions

- Now you were able to take over the user session. Imagine a situation where you would only get the
  callback when they log in. Why would even this information be useful for attackers?

```


```

- How can subdomain takeovers be prevented?

```


```

- What additional protections could an organization do to prevent abuse even if a subdomain takeover occurs?

```


```

## Additional Questions

Normally you could do subdomain recon via DNS queries to find domains that exist, but do not lead anywhere.

- Does the tool `nmap` have any useful scripts or plugins to find out (un)used subdomains for a site?
- What kind of arguments would you use to find subdomains for `example.com`?
- Are there any other tools or services to find out subdomains for a server?

```


```

Additionally, some good resources for domain discovery are __Passive DNS__  and __Certificate Transparency Logs__.
Research online what are they and how could you utilize them for subdomain takeover and summarize it in a few sentences:

```


```

A way to find out the hosting provider for a site is by seeing if it has a `PTR` record automatically configured by the
hosting provider in DNS.

What is a `PTR` Record?

```


```

Only looking at DNS data, can you tell who hosts the domain `ouspg.org`

```


```

(Optional) Take a look at the code for the [banking application](bank.py) and find out at least three major points where the
development has gone terribly wrong. Summarize in a few sentences to what type of attacks could the application be
vulnerable to or what major security flaws it has:

```


```

---

### Task 4: Non-Technical Alternative

If you cannot complete the technical exercises you can alternatively complete all of:

Task 1.A and Task 1.B
- Write further analysis on the effects of PSD2 on payment security for Task 3 (max 250 words)
- Write a short (max 500 words) analysis on the effects of emerging AI-technologies on online banking frauds and biometric authentication with at least two examples where it has already been used in frauds or other criminal activities.
- Summarize what is subdomain takeover and what measures can an organization take to protect itself from it (max 250 words)
