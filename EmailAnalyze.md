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
paypal accound to pay 9.99 few second ago, email was probably sended automatically from paypal.


I tried to reply for this mail and we can reply directly to this email without redirects.



Then I opened viev source to see better what is inside the email. 
I found a part of code with a link redirecting to the paypal page when clicking on "Afficher ou gerer le paiement"




I copied the link and checked on virustotal.com, resultats showed that link should be clean.



I didn't saw anything suspicious but as the last step I decided to check in google If paypal really has the service
with this address mail, and I found an article on offical Police web page that is confirmed that addresses emails
finishig by "@paypal.be" or "@s.paypal.be" are fake and is sure that is phishing.




## *Email_2*




