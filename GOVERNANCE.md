# Atlantis Governance

**Atlantis** is committed to building an open, inclusive, productive, and self-governing community focused on creating a high-quality infrastructure orchestration system. This document governs the community and defines how it should work together to achieve this goal.

Atlantis follows a two-tier governance model. The higher tier comprises the Atlantis Steering Committee, which is responsible for the project's overall health. [Maintainers](#Maintainer), [Core-Contributors](#Core-Contributor), and [Members](#Member) make up the lower tier. They are the main contributors to one or more repositories within the overall project.

The governance policies defined here apply to all repositories in the runatlantis GitHub organization.

## Atlantis Steering Committee

The Atlantis project has a project steering committee consisting of 5 members, with a maximum of 1 member from any single organization. The steering committee in Atlantis has a final say in any decision concerning the Atlantis project, with the exceptions of deciding steering committee membership, and changes to project governance. See [Updating Governance](#Updating-Governance).

The initial steering committee will be nominated by the current maintainers of the project in order to ensure continuity of the project charter and vision as additional members come on board. Once the terms of the initial committee members expire, new members will be selected through the election process outlined below.

A list of the steering committee will be published once decided and voted on.

Any decision made must not conflict with CNCF policy.

The maximum term length of each steering committee member is two year, with no term limit restriction.

Voting for steering committee members is open to all current steering committee members and maintainers.

## Repository Governance 

The Atlantis project consists of multiple repositories that are published and maintained on GitHub. Each repository will be subject to the same overall governance model, but will be allowed to have different teams of contributors (“members”, “core-contributor”, and “maintainers”) with permissions and access to the repository. This increases diversity of people in the Atlantis organization, and also increases the velocity of code changes.

### Member

**Defined by:** Member of the Atlantis GitHub organization

Members are continuously active contributors in the community. They can have issues and PRs assigned to them. Members are expected to remain active contributors to the community. This affiliation only comes with the base permissions (triage-only) for the organization, so the requirements are fairly low. Adding new members has the following benefits:

- Encourages a sense of belonging to the community and encourages collaboration
- Promotes visibility of the project by being displayed on each member’s profile
- Demonstrated tangible growth of the community and adoption of the project
- Allows issues to be assigned to the user

#### Requirements
- Enabled two-factor authentication on their GitHub account.
- Have joined the Atlantis Slack channel.
- Have read the contributor guide
- Are actively contributing to 1 or more repositories in the Atlantis GitHub organization. Examples include:
  - opening issues
  - providing feedback on the project
  - engaging in discussions on issues, pull requests, Slack, etc.
  - attending community meetings
- Sponsored by 2 Atlantis members. Note the following requirements for sponsors:
  Sponsors must interact closely with prospective members, e.g., reviewing code/design/proposal, coordinating on issues, etc.
  - Sponsors must be core-contributors or maintainers in at least one OWNERS file within one of the Atlantis GitHub organizations.
  - Sponsors must be from multiple member companies to demonstrate integration across community.

Once you've met the requirements, do the following steps:

- Open an issue against the runatlantis/org repo
- Ensure your sponsors are @mentioned on the issue
- Complete every item on the checklist (preview the current version of the template)
- Make sure that the list of contributions included is representative of your work on the project.
- Have your sponsoring reviewers reply confirmation of sponsorship: +1
- Once your sponsors have responded, your request will be reviewed by the Atlantis Steering Committee

#### Responsibilities and privileges

- Have the ability to _moderate_ GitHub discussions
  - This includes editing and hiding comments, labeling and closing discussions, and selecting an answer (when applicable)
  - This does _not_ include editing the opening comment
- Have the ability to _triage_ GitHub issues and pull requests
  - This includes labeling, closing or re-opening, adding to projects, assigning, and adding reviewers
  - This does _not_ include editing or hiding comments nor creating, deleting, or modifying labels or projects themselves
- Responsive to issues and PRs assigned to them
- Responsive to mentions of subprojects they are members of
- Active owner of code they have contributed (unless ownership is explicitly transferred)
  - Code is well-tested
  - Tests consistently pass
  - Addresses bugs or issues discovered after code is accepted
- Members are welcome and encouraged to review PRs and proposals.
- They can be assigned to issues and PRs, and people can ask members for reviews with a `/cc @username`.

**Note:** Members who frequently contribute code are expected to proactively
perform code reviews and work towards becoming a *core-contributor* for the
subproject/repo that they are active in.

### Core-Contributor

Core-Contributors are able to both review and approve code contributions as well as 
help maintainers triage issues and with project management.

While code review is focused on code quality and correctness, approval is focused on
holistic acceptance of a contribution including: backwards / forwards
compatibility, adhering to API and flag conventions, subtle performance and
correctness issues, interactions with other parts of the system, etc.

**Defined by:** *Core contributors* entry in an OWNERS file in a repo owned by the
Atlantis project.

#### Requirements

The following applies to the part of the codebase for which one would be an approver in an `OWNERS` file.

- Member for at least 3 months
- Author of at least 3 substantial PRs to the codebase, with the
  definition of substantial subject to the lead's discretion (e.g.
  refactors, enhancements rather than grammar correction or one-line pulls).
- Exhibiting sound technical judgment through PR contributions
- Exhibiting sound technical judgment through PR reviews
- Sponsored by a Maintainer
  - With no objections from other Maintainers or Steering Committee
  - Done through PR to update the OWNERS file


#### Responsibilities and privileges

The following applies to the part of the codebase for which one would be a core-contributor
in an `OWNERS` file.

- Core-contributor status may be a precondition to accepting large code contributions
- Demonstrate sound technical judgment
- Responsible for project quality control via code reviews
  - Focus on holistic acceptance of contributions such as dependencies with other features, backward / forwards
    compatibility, API and flag definitions, etc
- Expected to be responsive to review requests (inactivity may result in suspension until active again)
- Mentor Members
- May approve and merge code contributions for acceptance
- Monitor Atlantis Slack (delayed response is perfectly acceptable), particularly for the area of your repository
- Periodically attend the recurring community meetings
- In general, continue to be willing to spend at least 5% of their time working on Atlantis (~0.25 business days per week)

Each repository's current list of core-contributors is published and updated in each repo’s OWNERS.md file.

### Maintainer

Each repository in the Atlantis organization are allowed their own unique set of maintainers. Maintainers have the most experience with the given repo and are expected to have the knowledge and insight to lead its growth and improvement.

New maintainers and subproject maintainers must be nominated by an existing maintainer and must be elected by a supermajority of existing maintainers. Likewise, maintainers can be removed by a supermajority of the existing maintainers or can resign by notifying one of the maintainers.

If a Maintainer feels she/he can not fulfill the "Expectations from Maintainers", they are free to step down.

In general, adding and removing maintainers for a given repo is the responsibility of the existing maintainer team for that repo and therefore does not require approval from the steering committee. However, in rare cases, the steering committee can veto the addition of a new maintainer by following the conflict resolution process.

Responsibilities include:

- Strong commitment to the project
- Participate in design and technical discussions
- Participate in the conflict resolution and voting process at the repository scope when necessary
- Seek review and obtain approval from the steering committee when making a change to central architecture that will have broad impact across multiple repositories
- Contribute non-trivial pull requests
- Perform code reviews on other's pull requests
- Ensure that proposed changes to your repository adhere to the established standards, best practices, and guidelines, and that the overall quality and integrity of the code base is upheld.
- Add and remove maintainers to the repository as described below
- Approve and merge pull requests into the code base
- Regularly triage GitHub issues. The areas of specialization possibly listed in OWNERS.md can be used to help with routing an issue/question to the right person.
- Make sure that ongoing PRs are moving forward at the right pace or closing them
- Monitor Atlantis Slack (delayed response is perfectly acceptable), particularly for the area of your repository
- Regularly attend the recurring community meetings
- Periodically attend the recurring steering committee meetings to provide input
- In general, continue to be willing to spend at least 25% of their time working on Atlantis (~1.25 business days per week)

Each repository's current list of maintainers is published and updated in each repo’s OWNERS.md file.

#### Removing a core-contributor or maintainer

If a core-contributor or maintainer is no longer interested or cannot perform the the duties listed above, they should volunteer to be moved to emeritus status. In extreme cases this can also occur by a vote of the maintainers per the voting process below.

## Conflict resolution and voting
In general, it is preferred that technical issues and team membership are amicably worked out between the persons involved. If a dispute cannot be decided independently, the leadership at the appropriate scope can be called in to decide an issue. If that group cannot decide an issue themselves, the issue will be resolved by voting.

### Issue Voting Scopes
Issues can be resolved or voted on at different scopes:

* **Repository**: When an issue or conflict only affects a single repository, then the maintainer team for that repository should resolve or vote on the issue. This includes technical decisions as well as team membership.
* **Organization**: If an issue or conflict affects multiple repositories or the Atlantis organizations and community at large, the steering committee should resolve or vote on the issue.

### Issue Voting Process

The issue voting process is usually a simple majority in which each entity within the voting scope gets a single vote. The following decisions require a super majority (at least 2/3 of votes). All other decisions and changes require only a simple majority:

* Updates to governance by the steering committee
* Additions and removals of maintainers by the repository’s current maintainer team
* Vetoes of maintainer additions by the steering committee

For organization scope voting, repository maintainers do not have a vote in this process, although steering committee members should consider their input.

For formal votes, a specific statement of what is being voted on should be added to the relevant GitHub issue or PR. Voting entities should indicate their yes/no vote on that issue or PR.

The votes will be tallied after a suitable period of time (the goal is 5 business days), and the outcome noted. If any voting entities are unreachable during the voting period, postponing the completion of the voting process should be considered.

## Updating Governance

This governance will likely be a living document, and its policies will, therefore, need to be updated over time as the community grows. The steering committee has full ownership of this governance and only the committee may make updates to it. Changes can be made at any time, but a super-majority (at least 2/3 of votes) is required to approve any updates.

## Credits

Sections of these documents have been borrowed from [Argoproj](https://github.com/argoproj/argoproj/blob/main/community/GOVERNANCE.md) and [Crossplane](https://github.com/crossplane/crossplane/blob/master/GOVERNANCE.md) projects.
