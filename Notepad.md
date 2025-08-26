## Buffalo Website update flow

1. Jeff syncs staging from prod
2. Commune reviews and applies updates then tests site functionality (various pages and job application flow)
    
    If anything is wrong Commune remediates or flags an update as an issue to research so we skip it in production
    
3. Jeff enables the ATS redirect
4. Jeff backs up production
5. Commune applies patches in production
6. Commune performs tests again in production


## Per LiquidWeb To see number of active connections

In that case you can do it by accessing the backend of the server(Command line interface) by running the below commands

To check the status of teh IP : csf -g ipaddress  
To unblock IP : csf -dr ipaddress  
To whitelist IP : csf -a ipaddress  


## Late this year

Monica improvement

- They write POs when they come back from a trip
    - Gets sent to vendor once details are decided
    - Then gets put into Celerant
- Could have an app that they enter the details and sends an email and writes to Celerant or makes an import file


Loren & Max
- Phishing training was allegedly allowed to be made mandatory.
	- We need a way to track completion of the email and web ones
		- Loren would like it by 12/1
- Revive the messaging alert
	- Anyone in IT needs to be able to send it
	- Loren want's us to be able to hit individual stores
- A tool to shut down all the stores in an area
	- Also for department
	- Also just individual stores


From CAC:
- Melissa want's a smaller laptop (she has a 16", they have 14")
- Area managers don't think we need to replace their laptops and the training tablets are good
- Area's will be reshuffling
	- We will get the list from Sabrina


8/26 - Loren & Brian
- Loren found some things in the event logs on the domain controllers and want's Brian to look into them
	- Loren will provide his screenshots
- Loren would like Brian to start checking event logs from time to time
	- I would recommend just making a schedule (vibes based isn't a good system)