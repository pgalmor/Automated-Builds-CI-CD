# **Automated Builds CI/CD**

I am Pol Galan, student of the [Bachelor’s Degree in Video Games by UPC at CITM](https://www.citm.upc.edu/ing/estudis/graus-videojocs/). This content is generated for the second year subject Project II, under supervision of lecturer [Marc Garrigó](https://es.linkedin.com/in/mgarrigo).


# What is QA?

The acronym means "Quality Assurance", which is a set of actions and programmed activities that are carried out on a game to ensure that it meets a series of quality rules, standards and requirements previously established by a QA department and the producers. This "quality" does not always mean that the game is good or that it will please the public, but means that has exceeded those parameters that the team and the company want.

To guarantee this quality, we use tests, which test the game, although QA encompasses many other processes apart from testing.


# QA as an agile process

The QA process is flexible and must be adapted to other teams, artists, programmers ... The process must be done throughout the project, specifically, since the first design document comes out we can start planning "what" and "how" we are going to test.

In order to evaluate each milestone and each build, we must first define a criterion for this, the QA department and the producers must make a document with the parameters that each team member must follow when testing, in addition to the specifications about how to make the report.


# Flowchart

![Flowchart](https://raw.githubusercontent.com/carlosredolar/QA-WORKFLOW/master/docs/flowchart.PNG)


# Test types according to the tester

- **QA Department testing:** a company team will check the game and the code for errors.

- **UX testing:** the game is tested by target users, which we expressly bring to analyze their reactions.


# Test types according to the methodology

## Automated tests

Automated tests are carried out by computers automatically, we can simulate thousands of behaviors to prevent or detect possible errors. Being done by a computer the processes are very fast and allow us to save time.

The most common tests performed through this process are:

- **Unit tests:** tests separate modules of code to isolate errors. Used mostly in core mechanics and database communication.

- **Resolution tests:** makes simulations of the game in different resolutions and simulating different devices to predict the behavior of the game in various scenarios.

- **Stress tests:** focuses on simulating strange and overloaded scenarios to find the limits of the game.

## Manual tests

Manual tests are carried out by people, the bad side of this is that people are slow and much less efficient than a computer, but the human factor makes us able to find errors about tastes and more complex improvements.

The most common tests performed by humans are:

- **Interface tests:** the equipment analyzes the elements of the interface, not only that it works correctly but also that it is as intuitive as possible.

- **Stress tests:** As we have clarified before, in stress tests we try to put our game to the limit.

- **Soaking tests:** is based on leaving the game doing tasks for a long time to see its reaction.

- **Sound tests:** This test not only checks that the sounds works, but also that all audios match the animations or give feedback on the joint aesthetics.

- **Mechanical tests:** it is checked that the mechanics work as they should and we give feedback on possible improvements.

- **Smoke tests:** is a short test in which we check the correct functioning of the game without pre-designing a test.

## Manual-automatic mix

In fact, companies that have a QA department use both methods and complement each other, while the automatic computer process is working on simple but very laborious tasks in a very short time, the human team is searching for errors that require more complexity.

## Tools to automate

To reach this mixed method we use tools that allow us to make manual work easier.
The main tool of every company is its own code, we create our own scripts that will allow us to test all kinds of things, implementation of "godmodes", "next level", "unlimited coins or lives" ...

There are also platforms that provide us with tools, such as Unity and its "Unity Test Tools" that allow us to do unit tests easily.


# Test Plan

The test planning focuses on the question "What are we going to test?" and "What resources do we need?". The test strategy is a document that details the processes and ways in which we will ensure that quality in our game. In this planning we define the testing process, the levels of tests, roles of each team member and each test defined in the plan.


# Test design

The design of the test is how the test will be carried out and the list of scenarios that we are going to cover.
To design the tests there are different approaches:

- **Proactive:** are tests that are designed as soon as possible, to more or less predict where we can find errors even before creating the build.

- **Based on risks:** are tests designed after the build to find errors in specific sites.


# Report

After each test, a report must be made to report errors and even successes.

The tools that companies usually use are: [Mantis](https://mantishub.com/?utm_source=google&utm_medium=cpc&utm_campaign=World%20Mantis%20Searchers&gclid=CjwKCAiA7t3yBRADEiwA4GFlI1svB4PN3PdMdcsKLbAbYFAPvWAloj_Br9gH8QK77PFNG_wnFl2rXxoC28IQAvD_BwE), [Jira](https://www.atlassian.com/es/software/jira?&aceid=&adposition=&adgroup=55901295097&campaign=1496094425&creative=407713566405&device=c&keyword=jira&matchtype=e&network=g&placement=&ds_kids=p35508006331&ds_e=GOOGLE&ds_eid=700000001550060&ds_e1=GOOGLE&gclid=CjwKCAiA7t3yBRADEiwA4GFlIx4zTKAMbLCLanfWbugxYiT3_9zkrmF3A6JLCJatlMRr3o95DMUtaxoCAlcQAvD_BwE&gclsrc=aw.ds) and [Google Docs](https://www.google.es/intl/es/docs/about/).

The most important part of the report is the format, which all team members must respect so that it is then easy for the programmer to understand and resolve the error.

- **Description of the error/bug:** brief description of the error.

- **Status:** current status of the error, whether it has just been detected, is being resolved, is resolved, or need not be resolved.

- **Step-by-step:** step-by-step description of how to get the error to occur.

- **Expected behavior:** description of how it should work without the error.

- **Relevance:** 3 types are grouped according to the importance of the bug. Type A for errors that affect the game experience. Type B for errors that affect the user experience. And type C for improvements in any field.

- **Priority:** here we declare how quickly we want to solve this error (if we want to fix it), not necessarily in the order of relevance, there may be minor relevance errors that we need to fix before.

- **Version:** we specify the version number or which build we are testing.

- **Platform:** we specify on which device we are running the build in which we have detected the error.


# Type of bugs

![bug01](https://raw.githubusercontent.com/carlosredolar/QA-WORKFLOW/master/docs/bug01.jpg)

In this image we can see that the opponent appears pixelated, therefore influences the user experience, but does not affect the game at all. It is a type B error that would have low priority because it would only occur with that enemy and for 2 seconds on the screen.

![bug02](https://raw.githubusercontent.com/carlosredolar/QA-WORKFLOW/master/docs/bug02.jpg)

In this image we see how the 3D modeling of the character has been altered, therefore influences the user experience, but does not affect the gameplay. It is a type B error like the previous one, but this one would have more priority because the user will have to deal with seeing this error during the whole kinematics or even part of the gameplay.

![bug03](https://raw.githubusercontent.com/carlosredolar/QA-WORKFLOW/master/docs/bug03.jpg)

In this image we can appreciate how after completing a mission the reward is exorbitant, therefore it directly influences the experience of the game and also the experience of other users as it is an online game. It is a type A error with maximum priority, because it can also affect the economy of the company if it affects microtransactions.


# Sources

[https://www.youtube.com/watch?v=UF3Ya0uvYpU](https://www.youtube.com/watch?v=UF3Ya0uvYpU)

[http://www.gamerdic.es/termino/qa/](http://www.gamerdic.es/termino/qa/)

[https://apiumhub.com/es/tech-blog-barcelona/ingeniero-qa-organizando-workflow/](https://apiumhub.com/es/tech-blog-barcelona/ingeniero-qa-organizando-workflow/)

[https://usersnap.com/blog/quality-assurance-workflow/](https://usersnap.com/blog/quality-assurance-workflow/)

[https://skywell.software/blog/qa-process-flow-in-software-testing/](https://skywell.software/blog/qa-process-flow-in-software-testing/)

[https://www.softwaretestinghelp.com/what-is-actual-testing-process-in-practical-or-company-environment/](https://www.softwaretestinghelp.com/what-is-actual-testing-process-in-practical-or-company-environment/)


# Contact

email: **carlos.redolar.torres@gmail.com**
