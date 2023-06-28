# Phishing Analysis

- Type of Challenge: Learning
- Duration: Two days
- Team challenge : solo


## Your Mission
As a SOC analyst, you have to analyze the 5 emails that your colleagues send you. 
You must determine which email appears to be phishing and write a report. 
Your report should include all your thoughts and print screens of all the tools you used 

## *Email_1:*

Recived from: service@paypal.be

I started my analize with looking at the mail. 
First I checked email address: service@paypal.be and it looked correctly, all big company's/organisation's/corporation's etc
have them own domenes, If here would be p.ex servicepaypal@gmail.com we could be sure that it was an email from private user,
not from paypal.
Next step was checking the time of the mail, It was send few second after payment, it means that if the user used his
paypal accound to pay 9.99 few second ago, email could be sended automatically from paypal.

![email1_1 jpg](https://github.com/OlgvP/Windows-Powershell/assets/133352245/f36638c3-ec22-41c4-87bd-0b9463f07a17)

I tried to reply for this mail and we can reply directly to this email without redirects.

![email1_2 jpg](https://github.com/OlgvP/Windows-Powershell/assets/133352245/3aa842e1-088a-4e45-b9dc-94f2e9d03a62)

Then I opened viev source to see better what is inside the email. 
I found a part of code with a link redirecting to the paypal page when clicking on "Afficher ou gerer le paiement":


![email1 jpg](https://github.com/OlgvP/Windows-Powershell/assets/133352245/9b9d9cd0-c8db-4c16-8de6-923e5dca531f)


I copied the link and checked on virustotal.com, resultats showed that link should be clean.

![Email1_3 jpg](https://github.com/OlgvP/Windows-Powershell/assets/133352245/0b40464d-4d1d-4492-8164-a7170505144c)

I didn't saw anything suspicious but as the last step I decided to check in google If paypal really has the service
with this address mail, and I found many articles, one on offical Police web page that is confirmed that addresses emails
finishig by "@paypal.be" or "@s.paypal.be" are fake and is sure that **is phishing!**.

![email1_4 jpg](https://github.com/OlgvP/Windows-Powershell/assets/133352245/ce28ae1d-074e-4bf7-a323-ab34d605d256)


## *Email_2*


Recived from: stainless@midnightmagicevents.com

At first sight we can see that the e-mail looks poor. The domain name "midnightmagicevents.com" doesn't compare with 
the content of e-mail and is sure that is not the domain of "trust wallet".
Source code has 16 lines and doesnt look like secure source. Botton "Go to verification" redirects to climovil.com

![email2](https://github.com/OlgvP/Windows-Powershell/assets/133352245/09cee6e1-da8d-409a-a8cc-abfec3936f98)

I checked climovil.com on urlvoid.com and virustotal.com and I recived following information:

![emai2_2](https://github.com/OlgvP/Windows-Powershell/assets/133352245/0b394339-23c1-4890-ab1f-ac26b55371b3)

![email2_3](https://github.com/OlgvP/Windows-Powershell/assets/133352245/5c9c57f5-6cc0-46b4-95af-873f5e5dc6e1)

![email2_4](https://github.com/OlgvP/Windows-Powershell/assets/133352245/aaec7620-299d-4a0d-b2e2-f0a3e8aa85ed)


As we can see this e-mail has nothing common with "trust wallet", addres ip 
of the server is from Mexico. On virustotal.com 1 security vendor flagged this URLas malicious. Information from Urlvoid.com 
showing us that is definetely not "trust wallet".
**Im sure that is phishing e-mail.**

## *Email_3*

Recived from: gq@80-78-255-128.cloudvps.regruhosting.ru

This mail is not from Tinder. We can see that address domain is from russia and is definetely not address domain of Tinder.
I checked source code the mail and if we click on botton "find out who" we are going to be redirect to "htt[p]://[bl]og.tulingxueyuan.cn/contradictedqm.php?utm_campaign=tpdjuresn
blog.tulingxueyuan.cn"

![email3](https://github.com/OlgvP/Windows-Powershell/assets/133352245/7461b36c-85c5-44e1-b6c6-20ede0ac74d2)

I checked the domain address on urlvoid.com.

![email3_1](https://github.com/OlgvP/Windows-Powershell/assets/133352245/e2fa76cc-0d1e-4af6-b244-3c52edd6ab8c)

I chceck the domain of e-mail and the link we are going to be redirected if we click on botton, on virustotal.com.
Both of them are full of notification: "Phishing", "Malware", "Malicious"

![email3_2](https://github.com/OlgvP/Windows-Powershell/assets/133352245/d4504709-21ea-42a0-b94d-41d78a3e62f2)
![email3_3](https://github.com/OlgvP/Windows-Powershell/assets/133352245/040a7beb-6868-466c-aa9b-69af90a3bfb5)

**This e-mail is phishing!**


## *Email_4*

Recived from: <babakingsouthmichael@gmail.com>

As first sight this e-mail looks like spam. Is poorly written and domain belongs to a private user (domain gmail.com is a domain for private users).
Before even look inside we see information that sender this e-mail is Dan Miller, 
I did fast research (google, facebook, linkednl, wikipedia) and I didn't found any Dan Miller working in 
the United Nations Special Representative for Disaster Risk Reduction (UNDRR).
Even the tittle of the mail: Re: RELIEF / COMPENSATION FUND OF $1,500,000.00 USD looks like responding mail (Re:),
not like a e-mail addressed to us.

![email4](https://github.com/OlgvP/Windows-Powershell/assets/133352245/6cc2408c-a39d-40b6-bab8-38931b93fcb1)



I found also the web page, that helps with this type of spam called  "419" scam (aka "Nigeria scam" or "West African" scam),
there is a link to the list with spam-mails: http://www.419scam.org/419-bl-b.htm and our mail "<babakingsouthmichael@gmail.com>" is there.

![email3_4](https://github.com/OlgvP/Windows-Powershell/assets/133352245/717b976a-d426-44e2-bc08-552fc47880ad)

The content of this mail is incredible. 
No one is never sending money to random people in the internet.

**This mail is phishing mail.**

## *Email_5*

Recived from: Ariana<newsmail@app9l.serenitepure.fr>
Sender: 	Ariana<news@app9l.serenitepure.fr>
Reply-To:   Ariana<news@aichakandisha.com>

<img width="1421" alt="Screenshot_2023-06-28_at_16 11 45" src="https://github.com/OlgvP/Windows-Powershell/assets/133352245/b762e402-90f7-4e61-b079-d959ecefd51d">
 
The domain name we recived this mail doesn't look secure, looks like a scam. We have 3 different mails addresses.
Address we recived this mail from is different than: 
the sender address and address we can reply for this mail. It is a first sing that it can be phishing.
After I opened the source code of this mail I checked where we are going to be redirected when we click on the botton "probeer nu gratis uit"

![email_5_2](https://github.com/OlgvP/Windows-Powershell/assets/133352245/d00848f2-656d-4eb7-85c3-a12e9a530db3)

I checked the link on virustotal.com and it detected phishing and malicious.

![email5_1](https://github.com/OlgvP/Windows-Powershell/assets/133352245/4f87e772-2c3e-41b4-b9c7-e930ca17f536)


**Im sure that this is phishing e-mail.**


