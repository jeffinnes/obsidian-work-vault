## Jeff Notes

- <a> tags should not be placed in a <button> element. Use either/or and style as needed.
    - Rule of thumb: If the click action will take you somewhere else as its main function it should be an <a>. If it is going to have an effect on that page as its main function it should be a <button>.
- To make forms accessible, and ensure labels are correctly associated with their input, each <label> element should have a “for” attribute with the same value as its <input>’s “id” attribute
- When scheduling a task for the first time it made the first due date 1 week later than the actual due date

![[/Untitled.png|Untitled.png]]

![[Untitled 1.png]]

  

- When an advocate uses the search to find tasks, but leaves the task dropdown blank, the app crashes. Any other dropdown seems to handle being unset though.
- On the Submit Task page:
    - I think it would be a little nicer of a UX if it was ordered by the due date from oldest to newest
    - Another nice to have UX would be a toggle that hides completed tasks
- Let’s still get the auto-scheduler wired up to the login action, but I actually like the idea of having this button for admins. But let’s change the words to “Schedule upcoming tasks”

![[Untitled 2.png]]

- I definitely think this app can ditch the narrow layout and go full-screen to give more room for all of the tables.

## Sam Notes

- Is there a way to make tabs on the dashboard or like a key to drop down, so you don’t have to scroll all the way down to the next section?
- On Dashboard can we add the Area Advocate next to the GA# or some where so we can easily see who is which area for auditing? (Or you can ignore this if I just go to the task log page)
- For the Task Log can we make it into a grid? The tasks names are long and blend together

![[Untitled 3.png]]