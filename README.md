# Junior Ruby on Rails test

In this test you will code from scratch part of a simple back-office app to manage a Colonies residence.

The questions may seem a bit vague. That's on purpose. We would like to see what you can come up with without too much guidance, and there is no single right answer. If you have doubts about what is asked exactly, make a decision and carry on. Don't hesitate to add comments to explain your thought process and choices.

Your code should work (obviously), but you're also expected to pay attention to code quality and design patterns, as if you were part of a team building a production app.

From one question to the next, you may have to modify code you wrote before. *Don't plan ahead, instead try to find the best solution for each question independently, and package each question's code into a single commit.*

You are not expected to work on UI design at all. No CSS needed, just basic markup.

Use whatever test framework you like. Only write tests when asked!

No need to deploy anything, your app should just run locally.

In case you run out of time or you're stuck, write some pseudo-code or a comment about what you think could be done.

When you're done, push your code to a GitHub repo and ping us!

## Setup

Create an empty Rails app with recent versions of Ruby and Rails. The database you choose doesn't matter. Your views will be rendered by Rails.

Make it a git repo, and commit.

## Question 1

Set up the following domain model:
- tenants that have an email,
- studios that have a name and a monthly price,
- stays that represent a tenant staying in a studio for a given period.

Set up database seeds with a few typical records, including stays spanning over several months.

Commit.

## Question 2

Make sure it's impossible for two people to be in the same studio at the same time.

Write the corresponding test(s).

Commit.

## Question 3

Tenants pay their rent once every month.

Create a page that displays a given stay's info and the list of all of the payments (past and future) for this stay.

For each payment, show:
- the corresponding month's name,
- the amount (which is the studio's monthly price prorated to the time spent in the studio that month).

Remember, no UI design needed.

Commit.

## Question 4

We want to be able to give discounts in percentage on a given time span to our tenants, for example: Linda pays 30% less on her rent from the 10th of April to the 5th of June.

Update the domain model accordingly.

In the view from question 3, display the discounted amount for each payment.

No need to set up any other route, controller or view to manage discounts, just update the seeds with examples.
