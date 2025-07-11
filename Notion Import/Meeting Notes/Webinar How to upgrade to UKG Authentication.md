---
Created: 2025-01-09T08:31
Last Edited Time: 2025-01-10T16:22
Type: Training/Personnel
Created By: Jeff Innes
---
# Goals / agenda

- Learn about how the upcoming UKG auth changes are going to impact our users so I can communicate it to the rest of the UKG committee

# Discussion notes

- Login screen will looks slightly different.
    - Will now allow username or email
- Passwords can no longer be expired base on set period
    - Specific users will be notified if their password is detected in a significant breach (determined by UKG)
- Users that lock themselves out due to failed logins will now be able to self serve unlock via email
- Password resets will now be via email magic links, no longer able to set security questions
- For roles with MFA enabled, MFA will now be adaptive. Meaning trusted devices and IP addresses will only get prompted every 90 days (maybe that was 30 days)
- We can now brand the login page. Wow Yay I guess.

  

For adaptive MFA can we still require every time for critical roles?

- Answered

Yogesh Rajaraman 09:49 AM  
Not possible but we have confidence in our systems to detect threats and put employees through the appropriate sign-in experience.  

  

Upgrade Processes

- UKG will provide a self-service upgrade tool
- We might need to make some firewall rule changes
- Should take 30 minutes to do the actual update
- See the Possible Changes slides
    - Vanity URL will be nice
- Default passwords will have to change so we will need to update our New hire email templates
- Technically employees don’t HAVE to have unique email addresses, but users that share emails will be able to access each others accounts.

  

Start the upgrade

- Should only take 30 min
- Users should save any work before we start
    - They will get notified
- Punches will be queued during the upgrade and saved immediately afterward
    - We should still do this after hours

  

After Update

- Legacy app will also not be usable, employees will be notified if they try to log in

  

When?

- Sometime in the next 90 days we will get information about our exact timeline.
- We will have 60 days to complete from that date.
    - If we don’t, UKG will eventually disable features and then auto-update the critical points without warning.

  

# Action items

- [ ] Find out how many ASMs are using their bufex email
    - [ ] Can we make sure intake processes has people use a primary email (HR Step)
    - [ ] Is HR doing anything when someone promos to ASM to set their
- [ ] Inbox