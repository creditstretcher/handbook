# Development
This section of the handbook is for the parts that are dev team specific. 




## How we use Trello
**Board seperation**

The Trello boards are separated by project. 

If there are any overlaps due to Project A and Project B needing to work together, cards are created in both of the boards.

**Naming and description of cards**

The name should be short and concise

The description of the card should if possible a user story. Example: *“As a user I need to be able to see an overview of my credit stretches so that I know the status of the credit stretches I have created”*

Otherwise make sure that the task is explained thoroughly enough so that another person will be able to understand it

**Position according to priority**

The highest prioritised task should be on top.

**Suggestions**

Everyone is can make suggestions at any time.

Suggestions are added as cards in the Suggestions & General column below the "do not delete / move" cards.

Suggestions include tings such as:
- New features
- Changes to our development process
- Topics to be discussed during the next meeting
- Any good ideas

Assign yourself to the card with your suggestion.

At the next meeting we will go through the suggestions.

### The Trello lists

**Backlog**

Cards that should be added to the product at some point, but aren't in the current scope of tasks.

**Todo**

The current scope of tasks, which are added the to product in the near future.

**Doing**

The tasks we are working on at the moment.

**Paused**

Tasks which are waiting for other parts to be completed before they can be finished. Tasks that are waiting on other parts and aren't in the current scope of tasks are placed in the Backlog and not in Paused.


**Completed tasks (but not ready for review)**

When a task has been completed but it is not yet in a pull request or ready to be reviewed

**Code Review (is in pull request)**

When a card has been completed and is in a pull request it is put in code review. 
The person(s) who should review the code should be assigned to the card.
If possible attach the bitbucket commit/branch/pull request to the card when its put there


### How we use Bitbucket


**When working on a new feature, always follow these steps:**
1. Create separate branch with a name that describes the feature main objective
2. All commits regarding the feature should be in this branch
3. Create pull request to master branch and assign at least one other college for code review
4. After the discussion of the vague parts of the code and fixing of issues merge your branch with master branch and delete this old branch

Note: The branch should be created for each feature which makes sense as a unit. So if the feature requires to implement something both on a server and a client side both parts should be included in this branch so after it is merged with master the application will not break and number of features will increase.



**Commit messages:**
Try to describe your work in concise way if possible, use the following tags so everyone knows what the commit is about:

FEATURE: means that the commit contains part of new feature which is going to be implemented within the branch, should be only used within feature branches

BUGFIX: means that you found an error in your code and you would like to fix it, the commit should contain only code that fixes the error, commit message should describe the incorrect behaviour of the software before the applying the bugfix

CLEANUP: means that you are cleaning up the code to get rid of the unnecessary things, like some console logging, hard-typed values, ... so on

REFACTOR: means that you want to improve cleanliness of the code and simply rewrite the part of file or feature to more clear, effective or concise

DESIGN: means that Christian has been doing his magic ;)

Note: The commit messages should be written in the following way:
TAG: message, so eg.: CLEANUP: removed console logging used for debugging

**Pull requests:**

- Make sure that you resolve the conflicts

- Make sure that you created sufficient test for implemented functionality

- Make sure that all the tests are passing

- Attach relevant people to review the code

- Update trello accordingly
