###### tags: `Technical Committee`

# Technical Committee Meetings 2024

[![HackMD documents](https://hackmd.io/badge.svg)](https://hackmd.io/sL9z7MGwSCOGSCXeY27mFg)

## Quick links

* [Logistics](#logistics)
* [Agenda and Notes](#agenda-and-notes)
    * [2024-02-01 Meeting](#February-1-2024)
    * [2024-01-25 Meeting](#January-25-2024)
    * [2024-01-18 Meeting](#January-18-2024)
    * [2024-01-11 Meeting](#January-11-2024)


## Logistics

* **When:** 13:00–14:00 CET, every even week on Thursdays
* **Where:** [Microsoft Teams Meeting](https://teams.microsoft.com/l/meetup-join/19%3ameeting_OTc1NDIzNTUtYzJiMy00OThiLTkwZDUtYTdkODVhOGNjYzI3%40thread.v2/0?context=%7b%22Tid%22%3a%2292e84ceb-fbfd-47ab-be52-080c6b87953f%22%2c%22Oid%22%3a%2249725723-aa8c-4dcf-b9d0-b974e8a25702%22%7d)
* **Meeting Agenda and Minutes:** https://hackmd.io/sL9z7MGwSCOGSCXeY27mFg
* **Community Repo:** https://github.com/eiffel-community/community

## Agenda and Notes

Please do not update the meeting agenda and notes directly on GitHub and instead use the document on [HackMD.io](https://hackmd.io/sL9z7MGwSCOGSCXeY27mFg) in order to prevent notes getting out of sync.

### Next

* Should we evaluate Eiffel against the [OpenSSF Security Scorecard](https://github.com/ossf/scorecard) and/or the [OpenSSF Best Practices](https://www.bestpractices.dev/en)?
* Should we enable Code scanning for all repos. See https://github.com/eiffel-community/eiffel-remrem-publish/security/code-scanning for an example.
    * Set via https://github.com/eiffel-community/eiffel-remrem-publish/settings/security_analysis
    * Workflow example: https://github.com/eiffel-community/eiffel-remrem-publish/blob/master/.github/workflows/codeql.yml
    * We need to understand how code scanning works before we enable it globally. Do we need a workflow similar to the codeql.yml above for things to work or is it enough to just click Enable in the repo (or global) settings?
    * When/if decided: Enable all code scanning, Dependabot, secret scanning etc globally from the organization and send email to the mailing list about this change.
* Eiffel Summit 2024: Where and when?
* TC elections

### February 1, 2024

#### Participants

* TC Attendees
    * Emil Bäckmark, present
    * Magnus Bäck, present
    * Mattias Linnér, present

#### Agenda and Notes
* Rollcall, All
    * We have quorum.
* Agenda Bashing, All
    * Approved.
* Action Item Review, All
    * Follow up [the TC GitHub project board](https://github.com/orgs/eiffel-community/projects/3/views/4)
    * Follow up [the Eiffel protocol project board](https://github.com/orgs/eiffel-community/projects/6)
* Updates from CDEvents, Emil
    * Ticket events are being discussed; creation, closure, and updates of tickets. See [github.com/cdevents/spec#180](https://github.com/cdevents/spec/pull/180).
* Should we propose to add event triggered updates to Renovate?
    * Note: Renovate has support for Gerrit now: https://github.com/renovatebot/renovate/releases/tag/37.112.0
    * Similar issue in CDEvents: https://github.com/cdevents/spec/issues/39
    * No action for now.
* Archiving stale repositories
    * We'll create an issue in each repository that we think should be archived and ask the ostensible maintainers to complain if they want the repository to remain in an active state. See [github.com/eiffel-community/eiffel-store#10](https://github.com/eiffel-community/eiffel-store/issues/10) for an example.
    * Candidates for archival:
        * eiffel-gerrit-lib
        * eiffel-gerrit-herald
        * eiffel-jenkins-plugin
        * eiffelactory
        * eiffel-persistence-technology-evaluation
        * ml-jmespath-generator
        * eiffel-vici
        * eiffel-jira-plugin
    * Decision: TC will take over eiffel-playground and turn it into a community repo.
* Out of time, postponed: Self-hosted GitHub runners
    * https://www.securityweek.com/major-it-crypto-firms-exposed-to-supply-chain-compromise-via-new-class-of-ci-cd-attack/  
    > To mitigate this class of vulnerability, organizations are advised to change the default repository settings so that all outside contributions require approval.
* Out of time, postponed: Open source tool for inserting events to MongoDB?
* Out of time, postponed: PRs and issues

#### Action Items
* Emil: Look into proposal made in the maintainer role presentation from the 2021 summit.
* Magnus: Ask the security officers to try out the private vulnerability reporting feature.
* All: Evaluate key repositories according to the OpenSSF criteria.
* ?: Read up on static code analysis (see item in Next) and bring info to TC
* Magnus: Look into why "Reply All" on Google Groups doesn't actually reply all.
* Magnus: Check the proposed name of the source code tag event against the proposed new source change events to see if they're reasonably well aligned. If so we can move on with the tag event without waiting for the source change events.
* ~~Emil: Send existing Volvo contacts an email and ask about a summit.~~
* Magnus: Write an agenda for the OTel meeting.
* Mattias: Draft text of email to maintainers re archival.

### January 25, 2024

#### Participants

* TC Attendees
    * Emil Bäckmark, present
    * Magnus Bäck, present
    * Mattias Linnér, present

#### Agenda and Notes
* Rollcall, All
    * We have quorum.
* Agenda Bashing, All
    * Approved.
* Action Item Review, All
    * Follow up [the TC GitHub project board](https://github.com/orgs/eiffel-community/projects/3/views/4)
    * Follow up [the Eiffel protocol project board](https://github.com/orgs/eiffel-community/projects/6)
* Updates from CDEvents, Emil
* Eiffel Summit 2024: Where and when?
    * There are two windows of opportunity: late April or early May or during the fall, e.g. early September.
    * Let's ask Volvo Trucks if they're interested in hosting a one or two day summit.
    * Action Emil: Send existing Volvo contacts an email and ask about a summit.
* Community meeting Feb 15
    * Decision: OpenTelemetry and Eiffel, hosted by Magnus.
    * Action Magnus: Write an agenda for the OTel meeting.
* Should we archive all repos that don't have active maintainers?
    * Yes. Suggestion to send email to maintainers and check if they still consider themselves maintainers.
    * Action Mattias: Draft text of email to maintainers re archival
* Out of time, postponed: Should we propose to add event triggered updates to Renovate?
    * Note: Renovate has support for Gerrit now: https://github.com/renovatebot/renovate/releases/tag/37.112.0
    * Similar issue in CDEvents: https://github.com/cdevents/spec/issues/39
* Out of time, postponed: PRs and issues

#### Action Items
* Emil: Look into proposal made in the maintainer role presentation from the 2021 summit.
* Magnus: Ask the security officers to try out the private vulnerability reporting feature.
* All: Evaluate key repositories according to the OpenSSF criteria.
* ?: Read up on static code analysis (see item in Next) and bring info to TC
* ~~Emil: Send the appointed election officers an email to announce the appointment and request that they present the election timeline at the Feb 8 TC meeting. Also add them to the meeting invite.~~
* Magnus: Look into why "Reply All" on Google Groups doesn't actually reply all.
* Magnus: Check the proposed name of the source code tag event against the proposed new source change events to see if they're reasonably well aligned. If so we can move on with the tag event without waiting for the source change events.
* Emil: Send existing Volvo contacts an email and ask about a summit.
* Magnus: Write an agenda for the OTel meeting.
* Mattias: Draft text of email to maintainers re archival.

### January 18, 2024

#### Participants

* TC Attendees
    * Emil Bäckmark, present
    * Magnus Bäck, present
    * Mattias Linnér, present

#### Agenda and Notes
* Rollcall, All
    * We have quorum.
* Agenda Bashing, All
    * Approved.
* Action Item Review, All
    * Follow up [the TC GitHub project board](https://github.com/orgs/eiffel-community/projects/3/views/4)
    * Follow up [the Eiffel protocol project board](https://github.com/orgs/eiffel-community/projects/6)
* Updates from CDEvents, Emil
* Initiate TC elections by appointing Election Officers for 2024
    * https://github.com/eiffel-community/community/blob/master/GOVERNANCE.md#election-officers
    * Decision: Fatih Degirmenci and Fredrik Fristedt are appointed election officers until Jan 31, 2025.
    * Action Magnus: Update [GOVERNANCE.md](https://github.com/eiffel-community/community/blob/master/GOVERNANCE.md) accordingly. Draft issue created.
    * Action Emil: Send the appointees an email to announce the appointment and request that they present the election timeline at the Feb 8 TC meeting. Also add them to the meeting invite.
* When we answer someone who sends a mail via the Community Mailing list they need to be a member to see the response.
    * Action Magnus: Look into why "Reply All" on Google Groups doesn't actually reply all.
* Scope of [Santiago edition](https://github.com/eiffel-community/eiffel/milestone/9)
    * One issue added to the edition and the due date was updated to 2024-03-15.
* Can we add a source tag event ([github.com/eiffel-community/eiffel#219](https://github.com/eiffel-community/eiffel/issues/219)) before we're reasonably done with the new source change events?
    * Action Magnus: Check the proposed name of the source code tag event against the proposed new source change events to see if they're reasonably well aligned. If so we can move on with the tag event without waiting for the source change events.
* PRs and issues

#### Action Items
* Emil: Look into proposal made in the maintainer role presentation from the 2021 summit.
* Magnus: Ask the security officers to try out the private vulnerability reporting feature.
* ~~Emil: Talk to Panos about Vici's Dependabot PRs.~~
    * ~~We'll merge the Dependabot PRs now.~~
    * ~~Depending on whether or not we'll introduce a dormant state we'll transition the repo to either dormant or just archive it.~~
    * ~~Update 2024-01-18: Draft issue for archiving the repository has been created.~~
* All: Evaluate key repositories according to the OpenSSF criteria.
* ?: Read up on static code analysis (see item in Next) and bring info to TC
* ~~Emil/Magnus: Ask Fatih/Daniel/Kristofer and Fredrik if they're willing to be election officers for the next year.~~
* Emil: Send the appointed election officers an email to announce the appointment and request that they present the election timeline at the Feb 8 TC meeting. Also add them to the meeting invite.
* Magnus: Look into why "Reply All" on Google Groups doesn't actually reply all.
* Magnus: Check the proposed name of the source code tag event against the proposed new source change events to see if they're reasonably well aligned. If so we can move on with the tag event without waiting for the source change events.

### January 11, 2024

#### Participants

* TC Attendees
    * Emil Bäckmark, present
    * Magnus Bäck, present
    * Mattias Linnér, present

#### Agenda and Notes
* Rollcall, All
    * We have quorum.
* Agenda Bashing, All
    * Approved.
* Action Item Review, All
    * Follow up [the TC GitHub project board](https://github.com/orgs/eiffel-community/projects/3/views/4)
    * Follow up [the Eiffel protocol project board](https://github.com/orgs/eiffel-community/projects/6)
* Updates from CDEvents, Emil
    * Nothing in particular.
* Initiate TC elections by appointing Election Officers for 2024
    * https://github.com/eiffel-community/community/blob/master/GOVERNANCE.md#election-officers
    * Action: Ask Fatih/Daniel/Kristofer and Fredrik if they're willing to be election officers for the next year.
* Jan 18 community meeting
    * A possible topic for the community meeting on Jan 18 is OTel and how it might integrate with Eiffel (and vice versa). If we're not ready for that discussion by Jan 11 we'll cancel.
    * Decision: Cancel the meeting.
* We have multiple ongoing protocol PRs by multiple people. How can we work efficiently to avoid stepping on each other's toes and rebasing too much?
* Out of time, postponed: Scope of [Santiago edition](https://github.com/eiffel-community/eiffel/milestone/9)
* Out of time, postponed: Can we add a source tag event ([github.com/eiffel-community/eiffel#219](https://github.com/eiffel-community/eiffel/issues/219)) before we're reasonably done with the new source change events?
* Out of time, postponed: PRs and issues

#### Action Items
* Emil: Look into proposal made in the maintainer role presentation from the 2021 summit.
* Magnus: Ask the security officers to try out the private vulnerability reporting feature.
* Emil: Talk to Panos about Vici's Dependabot PRs.
    * We'll merge the Dependabot PRs now.
    * Depending on whether or not we'll introduce a dormant state we'll transition the repo to either dormant or just archive it.
* All: Evaluate key repositories according to the OpenSSF criteria.
* ?: Read up on static code analysis (see item in Next) and bring info to TC
* Emil/Magnus: Ask Fatih/Daniel/Kristofer and Fredrik if they're willing to be election officers for the next year.