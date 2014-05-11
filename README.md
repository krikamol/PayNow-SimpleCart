Sage Pay Now simpleCart(js) Shopping Cart Demo
----------------------------------------------

Revision 1.0.1

Introduction
------------

simpleCart(js) is a free and open-source javascript shopping cart that is very basic and simple to use.

This is Sage Pay South Africa's Pay Now third party gateway integration for simpleCart(js). This module gives you an overview on how to implement the Sage Pay Now gateway that will let you process credit card transactions. Sage Pay Now supports VISA and MasterCard.

Installation Instructions
-------------------------

Download the files from Github and extract them to a folder on your website, e.g. http://your_website/simplecart:
* https://github.com/SagePay/PayNow-SimpleCart/archive/master.zip

The files in the archive are described here:

| File/Folder        | Purpose                                             | Type |
| ------------------ | --------------------------------------------------- | ---- |
| index.html         | landing page for demo website                       | file |
| accept.html        | callback URL when transaction is accepted           | file |
| decline.html       | callback URL when transaction is declined           | file |
| no_javascript.html | page gets called if javascript not present          | file |
| js	             | folder with jquery and the two simpleCart libraries | file |
| images	     | four images to dolly up the website                 | file |

Configuration
-------------

Prerequisites:

To get this site working, you will need:
* Sage Pay Now login credentials
* Sage Pay Now Service key
* OpenCart admin login credentials

A. Sage Pay Now Gateway Server Configuration Steps:

1. Log into your Sage Pay Now Gateway Server configuration page:
	https://merchant.sagepay.co.za/SiteLogin.aspx
2. Type in your Sage Pay Username, Password, and PIN
2. Click on Account Profile
3. Click Sage Connect
4. Click on Pay Now
5. Click "Active:"
6. Type in your Email address
7. Click "Allow credit card payments:"

8. The Accept URL should be:
	> http://your_demo_website_simplecart_folder/accept.html
9. The Decline URL should be:
	> http://your_demo_website_simplecart_folder/decline.html

10. It is highly recommended that you "Make test mode active:" while you are still testing your site.

B. simpleCart Steps:

If you view source for index.html you will notice all the key Sage Pay Now fields being submitted, ie.:

*m1 - This should be your Sage Pay Now service key.
*m2 - Software vendor key which is fixed at 24ade73c-98cf-47b3-99be-cc7b867b3080
*p2 - Unique reference. *This should be unique on very submit to the gateway.**
*p3 - Description of goods
*p4 - Amount

The official technical documentation for simpleCart(js) can be found here:
https://github.com/wojodesign/simplecart-js

Demo Site
---------

The simpleCart(js) demo site will show you Sage Pay Now in action:
http://simplecart.gatewaymodules.com

Revision History
----------------

* 05 May 2014/1.0.1	Simplification and technical documentation added
* 18 Apr 2014/1.0.0	First version

Tested with simpleCart(js) version 3

Feedback, issues & feature requests
-----------------------------------

We welcome your feedback.
If you have any comments or questions please contact Sage Pay South Africa or log an issue on GitHub

