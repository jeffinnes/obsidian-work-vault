---
Created: 2024-07-30T16:59
Last Edited Time: 2025-01-15T11:31
Type: Internal Meeting
Created By: Jeff Innes
---
# 12/05/2024

## Goals / agenda

- Privacy
- Wallet
- App
- UKG Conference

## Discussion notes

- Privacy
    - Steve has a 23 page documentation on how to do the various ones.
    - Tyler will be the second level approver for the workflows
    - Since Tyler is included now they are going to go through a couple tests with the documentation to make any final reviews before going full force
    - HR still needs to determine how they will handle requests from people to know what info we have on them
- Wallet
    - Payroll has a portal and stuff
    - Linda will send out an email to the testers on how to get setup
        - We will then need to test some things
    - Likely to go live end of January
- App
    - Turn on so we can all test
    - Get full list of new features
    - PTO for Salary
    - Disable org chart and directory
    - Push notifications
    
- Conference
    - Big talk about AI tooling
    - Nothing officially new about Back office shutting down
        - Someone Tyler met learned that UKG has a team dedicated to it
    - Tyler took cool payroll classes
    - WFM
        - Implementation time is look like around a year maybe more
        - Base product
            - Time keeping and accrual
            - Some reporting
        - Add-ons we will need
            - A&P
            - Scheduling and Advanced Scheduling
            - Analytics module (maybe)
        - Target and Home Depot are using
        - They say we don’t have to have dedicated hardware
        - They will give us a UTM data dump but we have no idea what this will look like

## Action items

- [ ] Let’s turn on the feature to see pay stubs as soon as payroll posts
    
    Steve and Tyler will work together on that
    

---

  

# 10/22/2024

## Goals / agenda

- Mobile app
    - By December 31, 2024, UKG will automatically activate the new UKG Pro app for organizations currently using UKG Pro Classic and/or UKG Dimensions apps if they haven't already activated it themselves.
    - As of January 1, 2025, UKG will discontinue support, updates, and incident management for legacy apps (UKG Pro Classic, UKG Dimensions, and UKG Talk).
    - By March 2025, all legacy apps will be removed from app stores, requiring all users to transition to the new UKG Pro mobile app to avoid potential performance and functionality issues.
    - Use Testing Role for other features?
- Mass Erasure
- Wallet?

## Discussion notes

- Mass Erasure
    - Single delete feature for Mass Erasure
        - Enter emp ID, add to purge queue, output UKG ready CSV
    - How often to do the delete?
    - Currently we have a backlog of thousands. We can only do 500 at a time. But it looks like we can do multiple per day.
        - Any limits aren’t known right now
    - Next steps are
        - Verify app
        - Run through process and finish docs
        - Figure out frequency
        - Decide how to do approvals
    - Steve will work out the next part with HR
- Wallet
    - Waiting to get admin portal
    - There is no way to get notified of consent of direct deposit
    - Dec rollout is in question because UKG is slow
    - Will need to update the Direct deposit language
- Tyler will dig in a bit on WFM while at the conference
- Mobile App
    - Turn on app with basic features
        - We want to test Salary only PTO
    

## Action items

- [ ] Check out Virtual UKG Conference agenda

---

  

# 6/14/24

## Goals / agenda

## Discussion notes

Reviewing status of privacy manager

Steve presented his project plan for the Privacy Manager workflows

Sabrina is sure that we can’t hold any identifiable info so there really isn’t a reason to maintain an audit DB for the downstream automation processes

Payroll should test their reports after the first purge

Payroll will also need to look at purging their physical records

Steve and Amy added the supervisor field so it can be edited in the web portal

Now it can be set during intake

No longer need back office for this 🎊

Steve talked about some training he did - Tyler also did it

Not sure why he brought the packet from the class though, I missed what he said about that

Tyler has been working on moving as much to portal from BO as possible

UKG Wallet

Linda has reviewed all of the contracts and is working with lawyers

It’s possible that Linda will have contracts ready for RB to review soon

Linda mentioned this is an API integration. what?

**This is a UKG integration that’s already built I’ll just need to help wire it up**

New PTO Code

They are looking at buttons being redeemable for PTO

Before we will do a sandbox we need to create a laundry list of process improvements

Next meeting will be called by Steve/Jennifer. This will be a remote meeting unless in-person is justified.

## Action items

- [x] Reach out to UKG Rep about status of the new app
- [ ]

---

  

# 3/15/24

## Goals / agenda

## Discussion notes

- Reviewed the meeting Steve and I had
- Steve and Amy were trying to turn on editing for new hire workflows
    - Also there is an issue where when someone promo transfers to mgr, their pay sometimes changes back to ASM
- Payroll is working on looking into Wallet but they are being met with silence, they’ll push again
- Everyone has been migrated to the new final pay process
- HR has a Privacy Policy that is now posted to the UKG homepage
    - It is compliant federally and CA
    - Jennifer will look into figure out if CA needs to be purged after a certain date
- Steve is going to set up a Community tour with Katie

  

Next meeting, tentative for May.

## Action items

- [x] Steve and Jeff need to review the policy and start figuring out how internal workflows should/could work
- [x] Go ahead and set up a demo for UKG talk

---

  

# 1/19/24

## Goals / agenda

- Go ahead with CSP for all of HR and Payroll staff?
- What are our goals?

## Discussion notes

- Privacy Info Stuff
    - HR needs to set up a policy (they will work asap)
    - Once we have the policy we can determine workflows and what roles need to be assigned to whom
    - Probably should get a meeting with UKG on how to implement that
- Backoffice
    - Tyler has been auditing back office and making a list of things he wants to do in the web portal
    - He and Amy will consolidate lists and then they and I will get together and turn them on
- New hire/rehire mid-workflow edits exist and could be turned on HR will decide, might need to help with this
- App notes
    - In classic, could update tax forms not in new one?
    - Where does that news and info section of the app come from?
- UKG Talk, need an employee suggestion box, turn off features for self set up groups and one to one chat

## Action items

- [x] Janelle and Laticia can have support request everyone else in UKG can have UltiUniversity

App

- [x] Turn off Directory, and org chart and punches

---

# 1/19/24

## Goals / agenda

- Getting these going again after like 3 years
- UKG Conference findings?

## Discussion notes

- We should probably look back through past year of releases to see if there is anything we would want to turn on.
- WFM is actually integrated with Pro
    - Has some pretty nifty features that would work for how we do A&P
    - Features to generate docs based on workflow (like LOA?)
    - Linda: Let’s get a demo. Sabrina: yes but in Q3
- Linda is also looking at UKG wallet for early funds access, and some stuff about final pays
- We will need to look at turning on and testing the new app
    - Old app retires in may
    - New app fully released in January
    - There is a webinar on the new app from October in the community somewhere
- Platform config for intake and such that could be making the process better
    - Tyler is going to dive into it and see what’s up
    - For example we might be able to disable direct deposit
- UKG wants Back Office to go away in 2025
    - Next meeting we’ll go over the list of what everyone is doing in Back office
- Let’s get all of payroll and hr in CSP
- Privacy policy need to be developed
    - CA just passed a bunch
    - Other states are passing things
    - Pro has a privacy manager tool
        - Need to learn about it before turning it on
- UKG Wallet
    - They talked to some people and secured a promise of a reference

## Action items

- [x] Get with Stephanie and set up a demo on UKG talk as a replacement on Connecteam
- [x] Turn on new app in January
    
    [https://community.ukg.com/s/pro-mobile](https://community.ukg.com/s/pro-mobile)
    
    New app and classic share role settings
    
    Does not seem to be a way to limit access to New app while evaluating
    
- [x] Help find emerging privacy policy video for HR