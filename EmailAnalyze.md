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
finishig by "@paypal.be" or "@s.paypal.be" are fake and is sure that *is phishing*.

![email1_4 jpg](https://github.com/OlgvP/Windows-Powershell/assets/133352245/ce28ae1d-074e-4bf7-a323-ab34d605d256)


## *Email_2*




