Repository - helidon - analysis
https://github.com/helidon-io/helidon

Q1. The helidon project is a set of Java Libraries for writing microservices. It supports two programming models: Helidon MP (MicroProfile 5.0) and Helidon SE, which provides a small, functional-style API. The project aims to provide a framework for building microservices in Java. The repository has a history of development and has been active for several years (first release Sep 15, 2018). It currently has a total of 2,855 commits in the main branch and has attracted contributions from 73 collaborators.

Q2. The commits are very disorganized, in fact, only a few amount of commits have a title which start with a descriptive word such as add, upadrage and restore. The rest are all very consfusing, not detailed enough, making it difficult to navigate threw and understanding the scope of the commit before analysing it further. I would say that the users generally do not follow good formatting, lowering the general quality of the repository.

Q3. The repository have some good practice format but could be improved. We can divide the issues into four categories, each as important.
-Titles: Although the issue titles are generally concise, some could be more concise.
-Versioning: Version numbers are included in the titles and are helpful for identifying affected versions and prioritizing issues, these are not always present though.
-Labels: Labels are used for categorization and prioritization, they can differentiate between bugs, enhancements, or documentation updates, and indicate their priority levels (low, medium, high), thus improving overall organization.
-Description: Comprehensive descriptions are not really present, this could e improved.

Q4. Yes, there are instructions on how to contribute to Project Helidon. The main ways to contribute are through discussion, reporting issues, and submitting code that can be summarized as such:
-Discussion: Join the #helidon-users channel and participate in discussions.
-Issues: Report an issue with details such as Helidon version, application type and steps to reproduce.
-Code: To contribute to code, first sign the Oracle Contributor Agreement (OCA). Then, fork the repo, fix an issue or create one and fix it, and create a Pull Request then wait for a response or review.
Additionally, contributors should follow the Golden Rule and adhere to the Contributor Covenant Code of Conduct.

Q5. The automated checks in the provided GitHub project include:
   Assigning Issues to Projects: The assign-issue-to-project.yml workflow automatically assigns newly opened or reopened issues to the "Backlog Triage" project.
   Creating Backport Issues: The create-backport-issues.yml workflow allows manual triggering to create backport issues based on the provided issue number and Helidon version.
   Release Process: The release.yaml workflow is triggered on push events to branches starting with "release-". It sets up the environment, executes release scripts, and uploads staged artifacts.
   Code Quality and Validation: The validate.yaml workflow is triggered on pull_request events, push events (excluding "release-" and "test-release-" branches), and workflow_call events. It includes several jobs for checking code quality and validating the project:
   Copyright: Checks copyright information.
   Checkstyle: Performs code style checks.
   Spotbugs: Performs static analysis using SpotBugs.
   Build: Builds the project and archives test results.
   Docs: Generates project documentation.
   TCK: Performs Technology Compatibility Kit (TCK) checks.
   Examples: Builds and verifies example projects.
   Archetypes: Tests project archetypes.
   Packaging: Builds and tests packaging options (JAR, JLink, Native-Image).

Q6.
Q7.
Q8. The license used in the Helidon repository is the Apache License, Version 2.0. The Apache License is considered a permissive open-source license. Here are some key aspects of the license:
 Permissions: 
 - Commercial use
 - Modification
 - Distribution
 - Patent use
 - Private use
 Limitations:
 - Trademark use
 - Liability
 - Warranty
