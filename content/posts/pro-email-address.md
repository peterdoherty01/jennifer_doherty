+++ 
date = "2019-11-18"
title = "Setup Your Professional Email"
slug = "pro-email-address.md"
tags = ["email","godaddy","netlify"]
categories = ["startup"]
+++

I've been meaning to setup a professional email for my website for some time now. My goal was to send and receive emails from this address via my gmail. So, I got around to it and decided to share how I did it. **

## Prerequsities

1. You'll need a web domain e.g. www.yourdomain.com from a provider
2. Email account e.g. gmail; I'll show you how to send email froom there with your new prf address

## Step 1: Go to your Domain Provider

I'm using GoDaddy for this example but it should be very similar steps for another vendor.

Within GoDaddy:

1. Go to Additional Products
2. Choose "Email forwarding" (Not email)
3. Enter your desired email e.g. myname@yourdomain.com
4. Enter the address that the emails are sent to e.g; myemail@gmail.com
5. Go to Tools and choose server settings
6. Grab the MX settings which should be like: mailstore1.secureserver.net, value 10 & smtp.secureserver.net, value 0

## Step 2: Configure your DNS settings in Netlify

I'm using Netlify but you could configure this in GoDaddy if they are managing the DNS.

1. Add record type: MX
2. Insert _smtp.secureserver.net_ into the value field
3. Set the priority value to 0
4. Add a second record type: MX
5. Insert _mailstore1.secureserver.net_ into the value field
6. Go back to GoDaddy and check the settings are correct by going to the email forwarding menu
7. Click on Tools
8. Click on Server settings where you should see _"Your MX records are correct"_
   
## Step 3: SMTP2GO

1. Go to [SMTP2GO](https://www.smtp2go.com/)
2. Activate account by confirming in your email
3. Note the username and password
4. Add a new domain: yourdomain.com
5. Note the new TXT and CNAME records; 
6. Go to the DNS managed by Netlify and insert the records

## Gmail

1. In your email client, send an email from your gmail address to your pro email address
2. If successful, go to setttings
3. Look for accounts and import
4. Go to send email as
5. Add your new pro email add
6. 

## Conclusion

With Godaddy email forwwarding, you've a professional email address matching your website. Moreover, you've saved at least 50 dollars per year.
