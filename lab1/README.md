**UNIVERSIDADE LUSÓFONA DE HUMANIDADES E TECNOLOGIAS**

# Software Engineering - Laboratory 1: 🥼 <br>*Agile Software Development - A User Story Slicing Exercise*

**OBJECTIVE**: In this exercise, you will learn to:
* Create optimal flows in a Scrum Board/Kanban board; 
* The standard story format and write a good user story;
* Understanding User Stories sizes using Story Points;
* User story estimation using Poker Planning with Fibonnaci voting system.

# Let's start with some theory 🤓

**What is a User Story?** 

One of the most important aspects of moving to Agile is understanding “stories”. It takes practice to write good stories, and this exercise allows you this practice. As the Product Owner, you must deliver your customer’s or stakeholder’s perspective and share with the project team what is needed and why.

User Story is a tool in which requirements are captured in an easy to understand plain language, and is written from the perspective of an end user. 

A user story must provide value to some user. An Agile process is driven by the completion of stories, each of which provides tangible, demonstrable value to the user/customer/stakeholder. A sprint consists of a set of conscientiously prioritized stories. Experience will show that it’s best to use a format for each story that identifies who the user is, what they need, and for what purpose (the why). Such stories are written in this format:

```
“As a ____, I need a ____ in order to ____”.
```

or 

```
As a < user > 
I want to < perform an action > 
So that < I expect…. > 
```

* The **who / user** in a user story could be someone with a particular functional role, who holds a certain title in the application software, comes from the perspective of a persona, or embodies the needs and behaviors of a hypothetical user. – “As a net banking customer”;

* The **what / perform an action** in a user story details in specific terms the need, feature, or functionality desired by the who. This is what your project team will build into the product or service. – “I want to add beneficiary in my account”;

* The **why / I expect** in a user story states the outcome and desired value. The user expects out of the action performed – “so that I can transfer money to the added beneficiary”.

Here’s an example of a user story that clearly defines the who, what, and why:
* *“As a jazz fan, I need a tuning knob in order to find a jazz station on the radio that I will enjoy listening to.”*.

User stories, based on the estimated size, are taken for implementation in an iteration. User stories should be granular enough that they can be completed within an iteration and cannot be continued in the following iteration. If a story cannot be completed within an iteration, the same should be split logically. User stories are prioritized by the product owner based on business priority and are available at the top of the product backlog. The dev team pulls the stories into an iteration backlog and implements them. The [Definition of Done(DOD)](https://www.scrum.org/resources/blog/done-understanding-definition-done?gclid=CjwKCAjwm8WZBhBUEiwA178UnFiFqICker4elVMX5oMU_LN-3V9opm5QzyoaX2zMIiFIRYlhl0MOwxoCZ5UQAvD_BwE) for user stories is decided by the team which includes acceptance criteria, and processes that need to be followed like unit testing, regression testing, code review, etc. The story is said to be “done” only when it meets the preset Definition of Done. 

**Keys to a Valuable User Story**
* Product Owners must have courage to ask for what they believe their users/customers/stakeholders really want.
* A story must have value to someone. It must make the product better in some way.
    * The story when complete will make a real-world task faster, better, easier to understand, have fewer steps, or collect better info;
    * The high priority stories affect the most users or procure the highest value dat;
    * Avoid exotic/one-off stories (i.e. edge cases).
* “Clean up the bugs we introduced in the last sprint” is NOT a user story because it does not add anything to the product.
* Remember the INVEST model! Good user stories are:
    * **I**ndependent - User stories should be independent of other stories. There should be no overlap between them. They can however follow one after the other in a sequence, in a way that makes it easy to schedule and implement them;
    * **N**egotiable - The story should not be written in so much detail that it becomes a requirement document. If it is in too much detail, it does not give an opportunity for the dev team to have any conversation with the product owner or the business. The story should be written with just enough detail so that it paves the way to open discussions with the product owner or business, and helps to elicit details or come up with creative solutions. By negotiating on the story with the relevant stakeholders, teams can come to a common understanding;
    * **V**aluable - The story should be valuable to the customer. It should clearly state why we are doing this? How is it going to produce value to the customer? What value will the customer realize by implementing this story?
    * **E**stimable - The user stories should have sufficient detail for the dev team to understand and estimate them. The conversation in 3 C’s helps the team to uncover the details with the product owner and stakeholders, so that they can size the story. If the story is too big and not sizeable, then the story should be refined or decomposed further. Whatever information the team may require should be available in the story for them to estimate it. In case there is a part of the story where the team has to do research, then a “spike” story may be created while the rest of the story can be estimated and taken for implementation;
    * **S**mall and - Good user stories should be small. This does not refer to the size or number of words written in a story. A small story is of the right length so that the implementation team can complete the story within an iteration. It should be small enough that the story is “fully delivered” during an iteration;
    * **T**estable - Testable – A good user story should be testable in order to be “Done”. This is supported by the “Confirmation” in 3 C’s where the team comes up with acceptance criteria for every story after the detailed conversation with the stakeholders. 
        * The customer should be clear about what he should test during the review. If he is not clear, then the story is not good enough to be implemented.
        * The team works together in a collaborative way to INVEST in good stories. The team learns to write good user stories as they work together and also proactively think about the values and criteria that are laid out in INVEST. 

**Types of User Stories**

We can classify user stories into functional and technical types: 

* **Functional** – Normally, a user story is written based on the functional aspects of the application software, while focusing on the user and the value of the functionality provided to the user. Functional stories concentrate on the product features which the customer will be testing at the end of an iteration based on the acceptance criteria defined for the story. 

* **Technical** – Technical stories are written to be able to support the functional stories. Technical stories can be classified as:
    * **Infrastructure stories** – any infrastructure addition/modification that may be required to support the functional story;
    * **Refactoring** – this type of story is written to maintain the code and address technical debts. This can be used for designing and automation needs as wel;
    * **Spikes** – stories that require research on architecture and design which may in turn help achieve the functional need of the custome.

**Example of User Stories**

Let us see some examples of user stories (Epics, Features and User Story) in this section. 

| ID | Epics |
|---|---|
| E1 | As a Sales Professional, I want to generate reports so that I can take a decision on the marketing strategy for the upcoming quarter |
| E2 | As a Banking Customer, I want to access net banking, so that I can access my account and make transactions |
| E3 | As an Administrator of the software, I want to access master records so that I can make changes to customer data |

| ID | Features |
|---|---|
| E2F1  | As a Banking Customer, I want to access Savings account so that I can view/make transactions |
| E2F2  | As a Banking Customer, I want to access Credit Card page, so that I can view and make transactions |
| E2F3  | As a Banking Customer, I want to access Loans page so that I can view my loans |
| E2F4  | As a Banking Customer, I want to transfer funds, so that I can move my funds to different accounts within my bank and other banks |

| ID | User Stories |
|---|---|
| E2F1U1 | As a Banking Customer, I want to access/view summary of my savings account, so that I know my balance and other details |
| E2F1U2 | As a Banking Customer, I want to Login to Net banking so that I can view credit card details |
| E2F4U1 | As a Banking Customer, I want to transfer funds within my own accounts so that I can move some balance across my accounts |
| E2F4U2 | As a Banking Customer, I want to transfer funds from my account to another account in another bank, so that  I can send money to my family and friends who have accounts in other banks |
| E2F4U3 | As a Banking Customer, I want to add beneficiary to my account, so that I can transfer funds to the beneficiary |

| ID | Technical User Stories |
|---|---|
| E2TU1 | As a Net Banking Administrator, I want to have the customer’s data backed up so that I can restore it any time in case of issues |
| E2TU2 | As a Net Banking application, I want to shake hands with another bank using a specific formatted XML so that funds can be transferred based on the customers’ needs |


**Example of an Agile Planning Roadmap**

![image](./images/user_story_mapping.png)


**Summary in video format** 📼
In the following [link](https://www.youtube.com/watch?v=LEPLaYcdgeg) you can find video that summarizes all of the above concepts.

# Exercise - Part 1/4 (Requirements Gathering with User Stories) 🤿

**PRE-REQUISITES** 👓:
* Theoretical lecture and practical classes slide deck;
* Carefully read and comprehend the User Story concept as stated above;
* Create an account in [Trello](https://forms.gle/yTsVwecqnvaTNtWKA) you can use an existing account, university or personal email address;

**Let's start** 🏁:
1. Form a group of 2 to 4 students and give a funny name to your team;
2. Go to Trello and create a board with our team name;
    * Share the board with all team members and professors (p5617@ulusofona.pt - Pedro Perdigão & p5932@ulusofona.pt - Rui Santos);
    * Create a "To do" column and create a new card with:
        * Exercise Scrum Role - (Stakeholder(1-N), Product Owner(1), Technical Architect(0-N));
        * Our full-name;
        * Student number;

3. Brainstrom with your team for one of the following (or your own) systems: WhatsApp, Facebook, Google mail (or similar, MBWay, a computer game, a shop that sells custom-made shirts, Uber, Travel Agency (Booking/AirBnB), etc. Your team **must identify** the following items:
    * 1 epics;
    * 3 features for the related epic;
    * 10 user stories for each feature;
    * 2 technical user stories for each feature.

4. Before your team starts brainstorming the user stories, write down on a new Trello card one a sentence that briefly characterising the purpose/value of your system.

**Notes**:
* Do not brainstorm the same system as	any	of your neighboring	teams;
* Make sure your team has at least 2 roles (stakeholder & PO) - (better	3+);
* Make sure	that the 10	user stories fulfill the **INVEST**	criteria;
* Remember to keep them in the correct format: “As a ____, I need a ____ in order to ____”.

# Exercise - Part 2/4 (Estimating User Stories using Poker Planning with Fibonnaci voting system) 🗳️

Planning Poker is a consensus-based technique for estimating, mostly used to estimate effort or relative size of user stories in Scrum.

**Rules of the Game** 🎲

In Planning Poker Estimation Technique, estimates for the user stories are derived by playing planning poker. The entire Scrum team is involved and it results in quick but reliable estimates.

* Planning Poker is played with a deck of cards. As Fibonacci sequence is used, the cards have numbers - 1, 2, 3, 5, 8, 13, 21, 34, etc. These numbers represent the “Story Points”. Each estimator has a deck of cards. The numbers on the cards should be large enough to be visible to all the team members, when one of the team members holds up a card.
* One of the team members is selected as the Moderator. The moderator reads the description of the user story for which estimation is being made. If the estimators have any questions, product owner answers them.
* Each estimator privately selects a card representing his or her estimate. Cards are not shown until all the estimators have made a selection. At that time, all cards are simultaneously turned over and held up so that all team members can see each estimate.
* In the first round, it is very likely that the estimations vary. The high and low estimators explain the reason for their estimates. Care should be taken that all the discussions are meant for understanding only and nothing is to be taken personally. The moderator has to ensure the same.
* The team can discuss the story and their estimates for a few more minutes.
* The moderator can take notes on the discussion that will be helpful when the specific story is developed. After the discussion, each estimator re-estimates by again selecting a card. Cards are once again kept private until everyone has estimated, at which point they are turned over at the same time.

**PRE-REQUISITES** 👓:
1. Part 1 **completed**;
2. Watch the following [video](https://www.youtube.com/watch?v=TxSzo3lwwWQ);
3. Understand the rules of Poker Planning;

**Let's start** 🏁:
1. For Poker Planning use the following tool [link](https://planningpokeronline.com);
    * The Product Owner clicks "Start New Game" and will lead the Poker Planning session;
    * Give a name and choose a Fibonacci voting system;
    * Click invite players and share the game URL between your team members;
    * Wait that everyone to join the game lobby.
    * **Card values:** Do not make any agreement on the meaning of the value of each card.
2. Now perform a voting round per each user story you have written in the part 1/4;
3. Add the estimation value to the User Story Trello card - You can add the estimation value directly on the title or in the description of the card;
4. Evaluate our estimations and take conclusions.

**Notes**
* Refinement and slicing: Some user stories have things in common. Check if they can detect and separate them into other stories or slice stories into smaller stories.

# Exercise - Part 3/4 (Scrum/Kanban Board workflow, User Stories prioritization & Group U/S into Sprints) 🈺

A Kanban board is an agile project management tool designed to help visualize work, limit work-in-progress, and maximize efficiency (or flow). It can help Agile teams establish order in their daily work. Kanban boards use cards, columns, and continuous improvement to help technology and service teams commit to the right amount of work, and get it done!

1. **Visual Signals** — One of the first things you’ll notice about a kanban board are the visual cards (stickies, tickets, or otherwise). Kanban teams write all of their projects and work items onto cards, usually one per card. For agile teams, each card could encapsulate one user story. Once on the board, these visual signals help teammates and stakeholders quickly understand what the team is working on;
2. **Columns** — Another hallmark of the kanban board are the columns. Each column represents a specific activity that together compose a “workflow”. Cards flow through the workflow until completion. Workflows can be as simple as “To Do,” “In Progress,” “Complete,” or much more complex;
3. **Work In Progress (WIP) Limits** — WIP limits are the maximum number of cards that can be in one column at any given time. A column with a WIP limit of three cannot have more than three cards in it. When the column is “maxed-out” the team needs to swarm on those cards and move them forward before new cards can move into that stage of the workflow. These WIP limits are critical for exposing bottlenecks in the workflow and maximizing flow. WIP limits give you an early warning sign that you committed to too much work;
4. **Commitment point** — Kanban teams often have a backlog for their board. This is where customers and teammates put ideas for projects that the team can pick up when they are ready. The commitment point is the moment when an idea is picked up by the team and work starts on the project;
5. **Delivery point** — The delivery point is the end of a kanban team’s workflow. For most teams, the delivery point is when the product or service is in the hands of the customer. The team’s goal is to take cards from the commitment point to the delivery point as fast as possible. The elapsed time between the two is the called Lead Time. Kanban teams are continuously improving to decrease their lead time as much as possible. 

**PRE-REQUISITES** 👓:
1. Part 1 and 2 **completed**;
2. Understand the purpose of a board in Scrum/Kanban and it's components;
3. Have the Kanban board workspace in Trello created.

**Let's start** 🏁:
1. Together picture which states do you think it makes sense, while you are developing a feature, to be present visibly in the board columns and create those columns;
   * Ensure you predict undesired scenarios;
   * Comparing to a state machine can be helpful;
   * Ensure critical Scrum components are contemplated in this board;
   * Make usage of **labels** in Trello, they will be helpful for some organization 🤓
2. Take a look at the User Stories you created in Part 1 and define priorities, which stories should be done first, last and in between;
   * One way of doing this is to group US subjects as a whole and see from a higher level respective;
3. Now that you have the US grouped, it's time to ensemble the course of action through the weeks/months;
   * Think of Sprints as 2 weeks of work;
   * Remember when we talked about **labels**? 😉 Now it's a good time to put in practice;
   * Organize the cards in the board to be visible which are going to be done in the first Sprint. Assume you will start the first sprint in the time you are doing this laboratory;
4. Review the whole process until now and picture in the long term to see it gathers all requirements.


# Exercise - Part 4/4 (Which Agile methodologies would you use for the development of your Systems?) 🎁

**PRE-REQUISITES** 👓:
* Part 1, 2 and 3 **completed**;

Countless methodologies follow this Agile mindset like e.g. - Scrum, Kanban, Extreme Programming (XP), Lean Development and Crystal.

1. Prepare a brief PowerPoint presentation about one of the above methodology that covers the following points:
    * Summary of the chosen methodology;
    * The reason why your team would benefit from choosing that specific methodology; 
    * Advantages & Disadvantages of the chosen methodology.
2. After your presentation is concluded:
    * Create a new card in Trello with the following text: - (Methodology name ) - Presentation;
    * Open the new card and upload the presentation as an attachement;
3. Prepare to present to the class the outcome of your work;
4. The intire class will evaluate your work on a Poker Planning game with the scale of 1 to 5.


# Good Luck!! 🍀 
