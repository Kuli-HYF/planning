### Some thoughts/questions/input after first stakeholder interview:

#### Who is going to register the company?
- When the first employee or company owner joins the website, the company doesn't exist yet
- Do they start off by filling in the survey and enter the company name?
- Is the company object created after this?
- If the first CTA is to fill out the form instead of registering as a user, we run the risk of bogus companies being filed
- The user that fills out the form at first should always register the company's basic data: the name (and address -> if we want to make the map), ~~be it~~  at start ~~or at ending~~ in the form
- ~~If at the end, we create a big *ss content type at that point (I think)~~ 
- We can handle registration (I mean creating the company object in Strapi on the first steps of the form)(It shouldn't be one big form, but submit in steps)
- Glassdoor for example requires registration up front: https://help.glassdoor.com/s/article/Add-my-company?language=en_US
- I guess the user registration up front is a way to counter bogus stuff
- It would be indeed more user-friendly to not have the sign-up first, but just the query as something to lure users in
- How do we prevent users from creating the same company twice? For example: 'HackYourFuture', 'HYF', 'Hack Your Future'
- If we let it up to anonymous employees, what if the company owner doesn't want to be on the website?


#### How can we prevent misuse of the platform?
- Only company owners (check by email)
- Check employee's email (still have to be with the company)
- If the badges depend on a rating system, how can we prevent a disgruntled employee from giving the lowest score everywhere?


#### The questionnaire (for first data gathering):
- Starting points for now: 
- https://igvm-iefh.belgium.be/sites/default/files/downloads/39%20-%20Checklist_ENG.pdf
- https://assets.bbhub.io/company/sites/46/2022/01/Bloomberg-Gender-Equality-Index-Methodology.pdf
- Don't make the survey too long or a drag
- Don't make it too complex
- Questions should be relevant and useable to our rating system


#### The survey/rating system (on the website):
- The Belgian Institute For the Equality for Women and Men uses a system with 5 scores in their checklist: https://igvm-iefh.belgium.be/sites/default/files/downloads/39%20-%20Checklist_ENG.pdf
- We can use a similar approach to calculate the end result/general rating
- Using a game-like level up system, we can generate in-between badges or trophies as users go along answering the survey: for example the 'well balanced' trophy showing scales for male/female employer balance
- Trophies can be awarded for number of questions answered
- There should be some kind of feedback on positive scores as well as tips for improvement
- There should be a nice visual element for each of the trophies as well as fun descriptions
- Overall the survey shouldn't feel like a chore, but more similar to a game-like level up system
- Not a long list, but rather a new screen for each new part with some illustrations
- If we stick with the name Kuli, 'you are Kulified' could be a thing, like 'qualified'


#### How can we entice users/companies to participate?
- Get a high score
- Leveled badges
- Get a prominent place on the landing page
- Get a bigger portion of the landing page with a more highlighted description
- Become a featured company
- To be able to show companies on the page, we should at least have their logo, this should be provided in the survey by the user
- High scoring companies can unlock features like adding additional photos or other extra publicity for their company


#### If we manage to build all this, an extra can be the map (job-seekers part):
- Get the geo coordinates from the address
- Show a marker on a (Google) map from these coordinates
- When clicking the marker, show a popup with information about the company's score and badges (from the database)
- This could lead to a new company page with more detailed information
- Data could be shown in graphs
