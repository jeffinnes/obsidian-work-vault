Copy the below notes into the GitHub issue when done reviewing
## Bugs

- [x] #25
- [ ] There was a possible math bug on the Labor Calculator step of the Wizard, see comment below for screenshot
- [ ] Wizard confirmation > The Math on the Wizard confirmation page doesn't match the previous step or the spreadsheet
- [ ] Month Planning > The math isn't matching the math that was displayed in the wizard
- [ ] When I saved at the end of the Wizard, it popped an error that the plan couldn't be saved. I tried many times so I could troubleshoot, when I finally closed the wizard to see what else I could test, I found that it kept appending the staff list to itself on the Weekly Analysis page
	- I think that's what happened anyway
- [ ] Schedule Template > There is a bug in the math for the Available Hours calculation

## Needed Changes

- [ ] Staff Management > Let's flip Job Title Order (See the snip from the payroll scheduling app below)
- [ ] Staff Management > When a required field isn't filled in, the error message doesn't indicate what is wrong. (i.e. missing job title or name)
- [ ] Staff Management > After looking at some of the existing schedules, it seems that the stores are sorting their staff by FT/PT status and then the position hierarchy. We should replicate that.
- [ ] Staff Management > Leading zeros on the daily hours value are not being trimmed like they are for the hourly wage values
- [ ] Staff Management > The employee order seems to change when the "save changes" button is used, but refreshing the page restores the order.
- [ ] Wizard > Expenses Step > Make sure the inputs are in the same order as the current spreadsheet

## Suggestions

- [ ] Staff Management > Add the "Scheduled hours" like in the wizard
- [ ] New Month Wizard > Bring the Back, Cancel, Next buttons in line with the other button positions (if easily possible, not worth significant time)
	- [ ] Are the Add and Remove buttons supposed to be there for the Import Default Schedule step?
- [ ] New Month Wizard > Labor Calculator Step > Let's remove the radio button selectors from this step. (Unless they are needed in which case, maybe instructions are in order?)