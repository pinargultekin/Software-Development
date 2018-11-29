# Software-Development
Twitter News Platform Development
Emine P. Gultekin
Endicott College
Software Engineering ITS 550
Project Due Date: 05/22/2018















Contents
1	Purpose	3
2	Packaging	3
3	Documentation	3
3.1	Release Notes	3
3.1.1	Developments	3
3.2	Getting Started Guide Twitter Reporters	4
3.3	User Guide	4
4	Source Code Control System	4
4.1	Models of Operation	4
5	Development Environment	5
5.1	Code Review Requirements	5
5.2	Static Analysis Tool Requirements	5
5.2.1	Coding Standards	6
5.3	Dynamic Analysis Tool Requirements	6
5.4	Stakeholders Requirements	7
5.4.1	Journalist Requirements	7
5.4.2	Users Requirements	7
5.4.3	Twitter Requirements	8
6	Support	8
7	References	9




 
 
1	Purpose
While there are many social media platforms, Twitter has become known as the place where news is breaking, due to the live, real-time aspect of its product. News is now being uncovered in mere moments and tweeted by any person with a smartphone and a camera. Twitter is also used by many people who suffer from censorship. Media is not free in every country. Unfortunately, some countries restrict to access to the news or they only permit to publish biased news. Therefore, many people use Twitter to get and to share the reliable news. Current Twitter News tab only allows users to share news’ link with limited letter comment. Development of Twitter News section allows people to share their article or video freely without any counted letter limitation.

2	Packaging
	The Twitter application can be downloaded from Google Play, App Store, Blackberry World, and Microsoft.
	The Twitter application is compatible with Windows, Mac OS, Blackberry OS, Android devices, Windows devices and IOS devices.
	The Twitter application is supported by Windows 7, Windows 8, Windows 10, IOS 9 or later.
	Users can tweet via the Twitter website, Twitter application, or SMS (Short Message Service).
	Updates will announce via Twitter’s official account “@Twitter.”

3	Documentation
3.1	Release Notes
3.1.1	Developments
Version 8.0
	New user interface (UI) integration
	Column tab feature
	Tweeting without character limitation for approved journalists
	Location tagging feature for news/articles
	Topic tagging feature for news/articles
	News/articles can be viewed based on topic and location

Next Release Fixing – Version 8.1

	Live video sharing on News Tab will be fixed on next release.
	Adding “Favorite” icon for Tweets that user wants to save.

3.2	Getting Started Guide Twitter Reporters
	Apply to be Twitter Reporter
	Gather and upload required documents
	The Twitter completes the process within seven work days
	If a member is approved by Twitter, the reporter can start to tweet

3.3	User Guide
Available https://help.twitter.com/en/using-twitter
4	Source Code Control System
Source code control system (SCCS) is a software tool designed to help programming projects control changes to source code. [1] It provides facilities for storing, updating, and retrieving all versions of modules, for controlling updating privileges for identifying load modules by version number, and for recording who made each software change, when and where it was made, and why. [1] 
Source code control system divided into two; distributed and centralized. The concept of a centralized system is that it works on a client-server relationship. The repository is located at one place and provides access to many clients. [2] In a distributed system, every user has a local copy of the repository in addition to the central repo on the server side. [2] Distributed system provides some advantages such as flexibility, offline accessibility, faster, detailed change tracking – which means fewer conflicts at the time of merge. -, sharing changes with one or two teammates instead of sharing to everyone. The biggest advantage of distributes system if the main server’s repository crashes, every team member still have a local repository which helps to create the main repository. Popular distributed source code control tools are GIT and Mercurial. 
I prefer to use distributed system because of its’ reliability. It has a low risk for repository crashes. 

4.1	Models of Operation
Twitter uses GIT, due to its number of advantages. Also, I prefer to use the same model of operation for my project. It is amazingly fast, very efficient with large projects, and it has incredible branching system for non-linear development. [3] Unlike centralized version control systems, GIT branches are cheap and easy to merge. Feature branches provide an isolated environment for every change to member’s codebase. [4] Branching feature makes GIT reliable. GIT is used by open source projects because it is easy to leverage third-party libraries and encourage others to join one’s open source code. Therefore, GIT is compatible with my project.


5	Development Environment
5.1	Code Review Requirements
Code review is necessary for software development. When a developer is finished working on an issue, then the developer should look at whether the code does what it is supposed to do. Code Review, or Peer Code Review, is the act of consciously and systematically convening with one’s fellow programmers to check each other’s code for mistakes and has repeatedly been shown to accelerate and streamline the process of software development like few other practices can. [5] There are five different code review approaches which are formal inspection, over-the-shoulder, e-mail pass-around, pair-programming, and tool-assisted. Formal Inspection is a very formal type of peer review where the reviewers are following a well-defined process to find defects. [6] Over-the-shoulder reviews are the most common and informal of code reviews. [7] An “over-the-shoulder” review is just that – a developer standing over the author’s workstation while the author walks the reviewer through a set of code changes. [7] The biggest advantage of this review is simplicity in execution. E-mail pass-around reviews are the second-most common form of informal code review, and the technique preferred by most open-source projects. [7] Whole files or changes are packaged up by the author and sent to reviewers via e-mail. [7] Reviewers examine the files, ask questions and discuss with the author and other developers, and suggest changes. [7] the biggest challenge about this type of review is collecting the files under reviews. Tool-assisted reviews refer to any process where specialized tools are used in all aspects of the review: collecting files, transmitting and displaying files, commentary, and defects among all participants, collecting metrics, and giving product managers and administrators some control over the workflow. [7] Pair-programming is two developers writing code at a single workstation with only one developer typing at a time and continuous free-form discussion and review. [7] Studies of pair-programming have shown it to be very effective at both finding bugs and promoting knowledge transfer. [7]

5.2	Static Analysis Tool Requirements
Almost all software contains defects. [8] Some defects are found easily while others are never found, typically because they rarely emerge or not at all. Some defects that emerge relatively often even go unnoticed simply because they are not perceived as errors or are not sufficiently severe. [8] Static analysis tools are used to review code, searching for application coding flaws, backdoors or other malicious code that could give hackers access to critical company data or customer information. The primary advantage of static analysis that examines all possible execution paths and variable values, not just those invoked during execution. Thus static analysis can reveal errors that may not manifest themselves until weeks, months, or years after release. [10]
I choose Coverity for my project which fits best and supports project code language. It is also integrated with GitHub that provides quick and easy access. High level of accuracy analysis is the key factor why I choose Coverity as a static analysis tool for my project.
Coverity Static Analysis is a commercial product, and it pretends to be the leading automated approach for ensuring the highest-quality. [9] Because it produces a complete understanding of your build environment and source code, Coverity Static Analysis is a tool of choice for developers who need flexible, deep and accurate source code analysis. [9]


Benefits of Coverity Static Analysis:
	Automatically find critical defects that can cause data corruption and application failures
	Improve development team efficiency and speed time to market for critical applications
	Improve software integrity and end-user satisfaction [9]

5.2.1	Coding Standards
Coding standard is a series of procedure for a specific programming language that determines the programming style, procedures, methods, for various aspects of the program written in that language. Coding Standard is a very critical attribute of software development. 
Benefits of coding standards:
	Increases efficiency
	Minimize the risk of project failure
	Reduces complexity
	Easier maintenance
	Simplifies to locate and correct bugs
	Provides a comprehensive view
	Reduces the cost and development effort
 
5.3	Dynamic Analysis Tool Requirements
As I mentioned before, static analysis is the testing and evaluation of an application by examining the code without executing the application. Dynamic analysis id the testing and evaluation of an application during runtime. [10] The primary advantage of dynamic analysis that reveals subtle defects or vulnerabilities whose cause is too complex to be discovered by static analysis. Dynamic analysis can play a role in security assurance, but its primary goal is finding and debugging errors. [10] 
Features of dynamic analysis tools are as follows;
	To detect memory leaks
	To identify pointer arithmetic errors such as null pointers
	To identify time dependencies [11]
Intel Inspector XE is a dynamic analysis tool which does memory and thread checking and debugging. I prefer to use this tool because of its reliability and accuracy.

5.4	Stakeholders Requirements
A stakeholder is a person or organization that has rights, share, claims or interests with respect to the system or its properties meeting their needs and expectations. The interests of stakeholders have some influence on the project; therefore, their opinion should always be considered. The most important and obvious involvement for the stakeholder is during requirements development. This project’s stakeholders are;
	Owners of the Twitter: They vote on major decisions and serve as a source of financial accountability driving leaders to make a logical decision.
	Project Manager: Project manager uses his knowledge, personal and leadership skills help to achieve. 
	Development Team: They are responsible for planning, design, development, testing, and project delivery.
	Journalists: They are responsible for testing and using the application appropriately, giving feedback to the development team.
	Users: They are responsible for giving feedback to the development team.

5.4.1	Journalist Requirements
5.4.1.1	Functional
	A journalist can share photo, video, or article without letter limitation.
	A journalist can select if their Tweet personal or news by a different sharing button.
	A journalist can share news based on location by tagging.
	A journalist can choose a topic that news related with such as politics, economy, health, science, sports, etc.

5.4.2	Users Requirements
5.4.2.1	Functional
	The user can access current news without censor.
	There should be a new tab “Column” like a “News” tab, and users can read journalist’ article.
	News region can be put an order from general to specific like East America> New England> Massachusetts> Watertown. By doing so, the user can read or view regional news effectively.
	Each regions’ news (art, sports, economy) should be viewed separately.
	Recent news Tweets should be on the left side, and the news Tweets, which have the most interactions, should be on the right side.
	The user can see suggestions which match to user’s interest.

5.4.3	Twitter Requirements
5.4.3.1	Functional
	Twitter should provide a right to people who do not access the news from a regional news source.

5.4.3.2	Non-Functional
	Twitter must ask a journalist to provide documents that whether he/she is a journalist from authorized agencies.
	A Journalist must provide his/her documents twice a year from authorized agencies. Otherwise, his/her account is suspended.
	Twitter provides a microphone icon to his/her profile like authentication icon once journalist send his/her documents to twitter and twitter approved that he/she is a journalist. 
	Users can report journalist if they feel the news contains racism, sexism, abuse, or fake propagandistic information.
	The reports are examined, and if the journalist is guilty his/her account is suspended.

6	Support
If member experienced an issue on Twitter, she/he
	can upload a report through this link: https://help.twitter.com/en/contact-us
	or can tweet for 24/7 using her/his account.
	She/he can follow “@TwitterSupport” for the latest tips and tricks. 

7	References

[1] Rochkind, M. J. (1975) The Source Code Control System. IEEE Transactions on Software Engineering SE-1, No. 4, Pages 364-370.
[2] Retrieved from http://scmquest.com/centralized-vs-distributed-version-control-systems/
[3] Chacon, S. and Straub, B. (2018) Pro GIT. Mountain View: Apress.
[4] Retrieved from Atlassian: https://www.atlassian.com/git/tutorials/why-git#git-for-developers
[5] Retrieved from Smartbear: https://smartbear.com/learn/code-review/what-is-code-review/
[6] Retrieved from http://athena.ecs.csus.edu/~buckley/CSc233/Reviews_Types_Intro.pdf
[7] Retrieved from Northeastern University: http://www.ccs.neu.edu/home/lieber/courses/cs4500/f07/lectures/code-review-types.pdf
[8] Emanuelsson, P. and Nilsson, U. (2008) A Comparative Study of Industrial Static Analysis Tools. Retrieved from https://www.sciencedirect.com/science/article/pii/S1571066108003824
[9] Retrieved from Core: https://core.ac.uk/download/pdf/6552448.pdf
[10] Retrieved from Intel: https://software.intel.com/en-us/inspector-user-guide-windows-dynamic-analysis-vs-static-analysis
[11] Retrieved from ISTQB Exam Certification: http://istqbexamcertification.com/what-is-dynamic-analysis-tools-in-software-testing/
Retrieved from Intel: https://software.intel.com/intel-inspector-xe
Retrieved from Webguruz: https://www.webguruz.in/significance-coding-standards/
Retrieved from Carnegie Mellon University: http://www.cs.cmu.edu/~aldrich/courses/654/tools/cure-coverity-06.pdf
Retrieved from Coverity: https://scan.coverity.com/github
Retrieved from Vera Code: https://www.veracode.com/products/static-analysis-sast/static-analysis-tool
Retrieved from Twitter: https://help.twitter.com/en
Retrieved from Twitter: https://developer.twitter.com
Retrieved from Twitter: https://about.twitter.com/en_us/company/brand-resources.html
Retrieved from Twitter Community: https://twittercommunity.com/
Retrieved from Twitter: https://developer.twitter.com/en/case-studies/cbs-news
Retrieved from Twitter: https://twitter.com/Twitter?lang=en
