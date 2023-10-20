- [x] ABODE Designer Figma. Talk with Jason about it > Clarify with Michael what he wanted to do with ABODE in terms of the Designer thing.

- [x] WordPress Engine Keep the sites updated and also the plugins and bring up with the web team on any license issues. 
	- [x] Follow up with web team on license issues in wordpress engine

- [x] Check all of the plugins and research them for all the website and remove the unnecessary plugins that were possibly only used temporarily
	- [x] Read and make an organization of every plugin for the web team to choose which are to keep and remove.

- [x] Double check the Website, Figma, and Pitch Deck copy and compare to make sure all the property specs. for both SLiM and CAD3 are correct. 

- [ ] Organize all the emails in hello web email. Ask what to do with emails that come along to know what to do with each. 
	- [ ] Keep checking on the emails that come up.

- [x] Research on SPF record and DKIM, also DMARC
	- [x] Read on the general use case of these 2.
	- [x] Watch videos on these 2 things



- [x] App: Waiting Jason to update the slide for ABODE application.
- [x] WP: Waiting to move the sites ABD, ABODE, and ACCENT to WP Engine.
- [ ] Sites: Updating the sites currently in WP Engine. Web team needs to look into plugin license errors.
- [x] CAD3: Waiting to fix the new identified bugs in the site (everything is listed in Trello as comments). Also, Update the project specs for 321 WHYTE AVENUE, specifically the PROJECT COST & LUXURY AMENITIES. 
- [x] ABODE: Waiting for design sample in homepage that will include a new designer dashboard button. Also, new bugs have been found and is in Trello.


LATEST
- [ ] Ask about any updates present on any of the websites before updating it.
- [x] Distinctive Supply Figma -> Retrieve from Jason. (Pending)
- [ ] Distinctive supply has some design flaws that need to be checked. 
- [x] Accentuations, Abode, and Accent - Do not touch for any updates yet.
- [x] Ask customer support if the update for the plugin Elementor Pro can be deferred. (Cannot be deferred until its finished)
- [ ] In Smartsheet, put the plugins for each of the sites and checkout which can be removed. 
- [ ] Talk with the web team which plugins we can remove for each site. 
- [x] Get Hafstaff logo and put it as noreply@hellowriting.com (Pending)
- [x] Set noreply@hellowriting.com logo. Logos provided in Whatsapp by Fatima (Pending)
- [ ] Ask Michael if we can have access to the account of the domain provider for hellowriting.com to get started with setting up the SPF, DKIM & DMARC. (Pending)

- [ ] Setup the email authentication and security for noreply@hellowriting.com
- [ ] **SPF Record** - SPF helps prevent email spoofing by specifying which mail servers are authorized to send email on behalf of a domain. It works wherein the domain owner publishes a list of authorized sending servers (IP addresses) in DNS records. Receiving mail servers use this information to verify the sender's identity.
	- [ ] Login to the domain provider and locate the DNS
	- [ ] Within DNS, click add record and set type to TXT
	- [ ] Set Name into @ and in content enter "v=spf1 include:_spf.google.com -all"
	- [ ] Click save

v=spf1 include:\_spf.google.com -all
The syntax for the SPF record is like this by default. I can explain to you the structure of this text if you wish.

1. `v=spf1`: This specifies the SPF version being used, which is 1.
2. `include:_spf.google.com`: This includes Google's SPF record as part of your SPF policy. It allows Google's mail servers to send email on behalf of your domain, which is typically used when you're using Google Workspace for your email services.
3. `-all`: This specifies a strict policy that says all other servers (those not explicitly included in the SPF record) should fail SPF checks, and their emails should be considered unauthorized.

- [ ] **DKIM Record** -> May take 48 hours in order to be fully functional - DKIM adds a digital signature to email messages, allowing receivers to verify that the message hasn't been tampered with and that it genuinely came from the claimed sender. It works wherein the sender signs outgoing emails with a private key, and the recipient's mail server uses the sender's public key, retrieved from DNS records, to verify the email's signature.
	- [ ] Login to Google Workspace Account
	- [ ] Navigate to Apps > Gmail > Authenticate Email > DKIM authentication
	- [ ] Have the specified domain selected and click GENERATE NEW RECORD
	- [ ] Keep default values and click GENERATE
	- [ ] Copy DNS host name
	- [ ] Head back to your domain provider DNS
	- [ ] Within DNS, click add record and set type to TXT
	- [ ] Set Name into the Copied DNS host name
	- [ ] In Google Workspace Admin, copy the TXT record value
	- [ ] Paste the copied value into the record content and then save
	- [ ] Head back to Google Workspace Admin and then press START AUTHENTICATION

- [ ] **DMARC** - DMARC enhances email authentication by specifying what action should be taken for email that fails SPF and DKIM checks. It also provides reporting mechanisms for domain owners. It works wherein it instruct receiving mail servers to follow specific actions (e.g., quarantine or reject) for failed SPF and DKIM checks. DMARC also enables domain owners to receive reports on email authentication results.
	- [ ] Within DNS, click add record and set type to TXT
	- [ ] Set Name into \_dmarc
	- [ ] In Content, enter "v=DMARC1;p=reject;pct=100;rua=mailto:youremail;ruf=mailto:youremail;fo=1;aspf=r;adkim=r" and press save.


v=DMARC1;p=reject;pct=100;rua=\mailto:youremail;ruf=\mailto:youremail;fo=1;aspf=r;adkim=r
This DMARC syntax is something I personally made. I can explain the meaning of each jargon found in this text if you wish.

1. `v=DMARC1`: This specifies the DMARC version being used, which is just 1.
2. `p=reject`: This sets the DMARC policy to "reject," which means that any email failing DMARC checks should be rejected by the receiving mail server.
3. `pct=100`: This sets the percentage of messages that should be subjected to DMARC policy enforcement to 100%. In other words, all messages should be checked.
4. `rua=mailto:youremail`: This specifies the email address where aggregate DMARC reports (RUA) should be sent.
5. `ruf=mailto:youremail`: This specifies the email address where forensic DMARC reports (RUF) should be sent.
6. `fo=1`: This specifies the failure options. A value of 1 indicates that forensic reports should be generated and sent if both SPF and DKIM checks both fail.
7. `aspf=r`: This specifies the alignment mode for SPF (Sender Policy Framework). The "r" indicates that you are requesting strict alignment between the RFC5322.From domain and the SPF-authenticated domain.
8. `adkim=r`: This specifies the alignment mode for DKIM (DomainKeys Identified Mail). The "r" indicates that you are requesting strict alignment between the RFC5322.From domain and the DKIM-authenticated domain.


- [ ] Ask Michael if he has intentions of having all the sites contact info set to noreply@hellowriting.com (Pending)
- [x] Install CleanTalk for accentabd.com and accentuationsbydeisng.com
- [ ] Ask the Elementor Site if its possible to only purchase the Page Builder Plugin for 3 sites. (Pending)

follow up if they can connect the fandeck to the color reader app.




*Abawaze:* All done ✅
- [x] ~_Home Page:_ Replace restricted content navigation text with "Membership."~
- [x] ~_Packages Page:_ Remove all "USD pricings" and replace "Get Started" with "Contact Us."~
- [x] ~_About Us Page:_ Remove the word "clarity" in the subheading text below "WELCOME TO ABA WAZE."~

*Takeondaf:* Working 🟨
- [ ] _Display User Information Feature:_ Show users' names, location, and chosen Daf on the homepage.
- [x] ~_Functionality Change:_ Remove the starting count of 5000; numbers on the site should start with actual database values.~
- [x] ~_Website Issue:_ Investigate and resolve the critical error warning that may appear for multiple users.~
- [x] ~_Website Issue:_ Collaborate with the web team to investigate if the email received from the hello web email is related to the critical error warning.~
- [x] ~_Functionality Change:_ Disable the snippet feature in the site for form submissions and rename the snippet code for easy identification.~



