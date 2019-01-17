# <img src="http://www.rice.edu/_images/rice-logo.jpg" width=180> Comp427, Spring 2018, Homework 1
## Rational Paranoia
The homework specifications, as well as the corresponding course slide decks,
can be found on the [Comp427 Piazza](https://piazza.com/class/jqifhp864b37ju).
This assignment is due **Thursday, January 17 at 6 p.m.**

You will do this homework by editing the _README.md_ file. It's in
[MarkDown format](https://guides.github.com/features/mastering-markdown/)
and will be rendered to beautiful HTML when you visit your GitHub repo.

## Student Information
_Student name_: Ce(Calvin) Liu

_Student NetID_: cl104

## Problem 1- Scenario: Documents
- Assumptions:
  - The document management system has an authentication system that consists of different levels of security. It behaves in this way
    - Different People may have different levels of permissions. Each person has only one level of permission. For example, Alice has a level 1 permission. Permission with the large number has more access in this system than small numbers. 
    - Each file in this system also has a number associated with it.
    - The people with level x can only access(read and write) the files whose marked number are equal to or lower than x
  - The Document management system must support remote access. Since it is an international company, the company must have offices around the world. That means the employees around the world may need to access the files that are not stored in their local office. Therefore, the document management system must provide remote access features for the employees around the world.
    
- Assets:
  - The files themselves are the most important assets we need to protect. This consists of many aspects. 
    - First, it is very obvious that we need to protect the content of the files. 
    - Second, the names of the people who create and update the files are also the assets. The reason for this is that based on the description of the question, the files may contain political matters. In terms of the politics, even the names of the people who create or update some files that contain specific political views are leaked, the outcome could be catastrophic. 
  - The level of the permissions that people have and the level of the permissions that a file required to be accessed are also the assets we need to protect. 
    - First, they indicate what the level of the files are and what the level of permissions that a person has, which helps the system to grant or deny a person's access to a file. Therefore, they are assets.
    - Second, if we don't protect the level of the permissions, some people may change the permission they have so they can have a higher level of permission or decrease the permission level on the files so that anyone can access them. Therefore, they are the assets we need to protect.
- Threats:
  - The security crackers have the username and the password of an employee in this company so they can access the system.
  - The crackers find a system security bug to access the system without the username or password
  - The crackers intercept the data of the file transmission between different offices, like the man in the middle attack.
  - The crackers put some hidden software on the computer that the office just bought, so they can monitor what the employee read and typed.
  - The employees in the company may copy the files and leak them to someone else.
- Countermeasures:
  - Enable two-factor authentication feature. Even if the username and the password are leaked, they still can not log in to the account.
  - Only the computer within the company's network can access the database.
  - Before the transmission, encrypt the files. The name of the file must also be encrypted.
  - The computers in this company must only be bought from the stores which have a good reputation.
  - Put some hidden watermark on the files. The watermark should be made of the username who are accessing this file. Even if the files are stolen and leaked, the security person can still trace the source of the leak by the watermark. 

## Problem 2
- Scenario: Grading
- Assumptions:
  - Students turn in the assginments using Canvas.
  - TA starts to grade the assignments after the deadline.
  - TA grades the assignments by downloading the file and reviewing it. After I grade the assignments, I put the grade on Canvas.
  - After the grading is completed, TA make grade visible to students on Canvas.
- Assets:
  - The assignments that the students have are the important assets we need to protect. They are the intellectual property of students so they are assets. Besides that, the assignments shoubld be prevented from leaking becasue it is a violation of the Rice Honor Code and may make the privacy of students vulnerable. Therefore, we need to protect it. 
  - The students' grades are the assets we need to protect, since any leak of the grades with the students name are considered of the violation of the students' privacy. Therefore, we need to protect the students' grading. However, the distribution of the grading without the students' indentities are not considered as the assets that we need to protect. It is a assets of course because we can evaluate how much knowledge and how well the students have learned so that we can adjust what knowledge we should teach and how we teach them. But it is not the assets we need to protect because it is fine to open these data to the public. 
- Threats:
  - Some students may have the username and the password of some other students so that they can view other students' assignments as well as make some modification on the assignments. 
  - Some crackers may have the username asn the password of the TA's account so that they can view and change the grades of the students as they want.
  - Lots of the students turn in the assignments frequently right before the deadline that cause the server too busy to respond. In this case, the students may not be able to submit the assignment anymore.
  - When students use not secured wifi to submit the assignment, the assignment can be read by the crackers. If the crackers decided to share the assignment, it could lead to the violation of the Honor code and cause the students in trouble. The cracker can also modify the file uploaded that cause the student losing grade, which is very unlikely to be found, because usually the TA will not return the grading assignment therefore the TA and the students are not able to aware of it.
- Countermeasures:
  - Enable two-factor authentication feature and make it a mandatory step when students are trying to log in their accounts. 
  - Enable two-factor authentication feature and ask the TA to use it whenever he/she logs in.
  - Ask the students to submit the assignments early and limited the number of times that a student are allowed to submit in an hour when the final due is approaching. It could solve the problem but it also sacrafice the user experience. A better way to do it is by using Github. The TA can create an Github classroom proejct and ask students to submit it to the Github. Github has the ability to handle the submission of 200 students at the same time.
  - The students can choose to encrpt the assignment as well as using secure wireless network. Or they can use wired network to submit the assignment. The password to encrpt the assignment need to be shown to the students in the class.

## Problem 3
- Scenario: Gatekeeper of the company building. The gatekeeper controls who can enter the building. Only the people with proper ID are allowed by the gatekeeper to enter it.
- Assumptions:
  - The gatekeeper has the scan machine that can read the ID card and show that whether the person has the permission to enter the building.
  - The gatekeeper will follow his duty and will not be bribed to let someone in. 
  - This gatekeeper's duty are controling the access only at the frontdoor. Other doors are not in his duty.
  - The scan machine needs to connect to the company's wireless network to retrive the data from the database.
- Assets:
  - The scanner. It is the assets we need to protect. Without the scanner, the gatekeeper can not decide which person has the permission to enter the building.
  - The safety of the gatekeeper. 
  - The safety enviroment of the building.
- Threats:
  - Since the scan machine uses wireless network to  
  - explanatory_paragraph ...
- Countermeasures:
  - explanatory_paragraph
  - explanatory_paragraph ...

