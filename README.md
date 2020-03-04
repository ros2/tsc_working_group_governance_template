# {{NAME}} Working Group

{{
TEMPLATE: This repository acts as a template for individual Working Groups to start from.
All information in double curly-braces must be replaced with details for the specific Working Group.
NOTE: check the issue and pull request templates as well, under `.github` directory.

When starting a new working group, we recommend you fork this repository to the WG organization.
}}

This document defines the scope and governance of the Working Group (WG).

{{Mission: The {{NAME}} Working Group's mission is to...}}

{{Scope: the types of topics, tools, libraries, applications, documents, etc, that this working group focuses on. }}

## Subprojects

This Working Group owns and maintains the following Subprojects.
Its meetings and membership are largely focused on the direction, design, and work on the projects.

### Subproject List

The following subprojects are owned by the Working Group:

{{

* template-project
  * Description: Brief description of project. Remove this item and add new projects using this format.
  * Repositories
    * link-to-repository

}}

### Standards for subprojects

When adopting a subproject, the WG agrees that the following criteria will be maintained by the WG.

* Build passes against ROS 2 master
* The ROS 2 standard linter set is enabled and adhered to
* Builds have 0 warnings
* Quality builds are green (address sanitizer, thread sanitizer, clang thread safety analysis)
* Test suite passes
* Code coverage is measured, and non-decreasing level is enforced in PRs
* Issues are responded to promptly
* Releases go out regularly when bugfixes or new features are introduced
* The backlog is maintained, avoiding longstanding stale issues

### Adding new subprojects

To request introduction of a new subproject, add a list item to the "Subprojects" section and open a Pull Request to this repository, following the default Pull Request Template to populate the text of the PR.

At the next meeting, the PR will be reviewed, and merged on unanimous agreement from Approvers.

### Subproject changes

Modify the relevant list item in the "Subprojects" section and open a Pull Request to this repository, following the default Pull Request Template to populate the text of the PR.

At the next WG meeting, the PR will be reviewed, and merged on unanimous agreement from Approvers.

### Deprecating subprojects

Projects cease to be useful, or the WG can decide it is no longer in their interest to maintain.
We do not commit to maintaining every subproject in perpetuity.

To suggest removal of a subproject, remove the relevant list item in the "Subprojects" section and open a Pull Request in this repository, following instructions in the Pull Request Template to populate the text of the PR.

At the next WG meeting, the PR will be reviewed, and merged on unanimous agreement from Approvers.

If the repositories of the subproject are under the WG's GitHub organization, they will be transferred out of the organization or deleted at this time.

## Governance

### Meetings

* Regular WG Meeting: {{time schedule for meetings}}
  * {{when and where will meetings be announced}}
  * {{what artifacts will be posted after the meetings, e.g. Minutes, Recordings}}

### Communication Channels

{{How can members communicate with each other? Discourse, Discord, IRC, email list, etc.}}

### Backlog Management

{{Is any project management software/site used to track work for this Working Group? How can new members discover the highest impact tasks they could take on? GitHub Projects, ZenHub, etc.}}

### Membership, Roles and Organization Management

Working Group members may act in one or more of the following roles:

* **Member**
  * Prerequisite: Attend at least one out of the last three Working Group meetings
  * Responsible for triaging issues
* **Reviewer**
  * All reviewers are members
  * Prerequisite: A history of contributions to WG-owned Subprojects
  * Responsible for reviewing pull requests
* **Approver**
  * All approvers are reviewers
  * Prerequisite: A history of high quality code reviews on contributions to WG-owned Subprojects
  * Responsible for approving and merging pull requests
  * Responsible for vetting and accepting new projects into the Working Group
* **Lead**
  * TSC member or their delegate
  * Responsible for organizing and moderating working group meetings
  * Responsible for posting meeting materials (minutes, recordings, etc.)
  * Responsible for breaking ties

To become a member or change role, create an issue in this repository using the appropriate issue template.
Such applications are accepted upon unanimous agreement from Approvers,  and are typically based on the applicant's history with the subprojects of the Working Group.

### Modifying this governance document

Changes to this document will be made via Pull Request.
The PR will be merged on unanimous agreement from Approvers.
