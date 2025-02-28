# Project outline: MyHealtheVet to VA.gov notification preference migration

Last updated: October 5, 2022 

### Communications

- **Github labels**: vsa-authenticated-exp
- **Slack channel**: [#accountexp-authexp](https://dsva.slack.com/channels/accountexp-authexp)

### Roles

#### OCTO team

[This is managed by the VA.gov profile team](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/identity-personalization/profile/README.md#roles).

#### Stakeholders & Partners

|Name|Role|Email|
|----|----|-----|
|Carnetta Scruggs| MyHealtheVet management analyst| Carnetta.Scruggs@va.gov|
|Theresa Hancock| MyHealtheVet director| Theresa.Hancock@va.gov|
|Patricia Henry| MyHealtheVet program manager|Patricia.Henry@va.gov|
|Bresha Lipscomb| MyHealtheVet business analyst|Bresha.Lipscomb@va.gov|
|Ro Weaver|MyHealtheVet contractor|Rosanna.Weaver@va.gov|

### Table of Contents

- [Overview](#overview)
- [Problem Statement](#problem-statement)
- [User Outcomes](#user-outcomes)
- [Business Outcomes](#business-outcomes)
- [Measuring Success](#measuring-success)
- [Solution Approach](#solution-approach)
- [Backend](#backend)
- [Frontend](#frontend)
- [Design](#design)

## Overview

While most of the MyHealtheVet migration into VA.gov will take place in the health care "apartment", universal information, like the MyHealtheVet profile and settings, will move into the VA.gov profile. After completing [an audit of the MyHealtheVet profile and personal information sections](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/identity-personalization/profile/mhv-profile-research/recommendations.md), we learned that most of the information that exists in the MHV profile already exists in the VA.gov profile. However, MHV notification preferences are not yet supported by VA.gov, and are an essential piece of functionality that needs to move in to VA.gov. This engagement covers definition, collaboration with MHV, VA Profile, and VA Notify, and the build in VA.gov that will support the MHV notification preferences.

### Problems we'll tackle

**What notification preferences do we need to migrate**

We know we need to migrate the existing MHV preferences, but MHV has also mentioned other notifications they want to add in the near future. We will need to make sure each notification is defined so we can determine the right time to build a preference and/or to integrate the actual notifications through VANotify.

**Do we need to migrate all notification preferences at once, or can we take a gradual approach?**

As mentioned above, there are a handful of existing and new notifications/preferences that MHV are interested in having VA Profile and VANotify support. However, we will need to prioritize what gets integrated into VA Profile and VANotify and when based on the health apartment roadmap (notifications and preferences should be supported by the time a feature is supported on VA.gov), and MHV's long-term plan for their own profile.

**Do we need to migrate existing notification preference data from MHV to VA Profile? If so, is this possible?**

Given that we are working with existing notifications for which people have existing preferences saved, we'll need to talk to VA Profile about whether a data migration is possible or not.

**When do we need to integrate the actual notifications with VANotify?**

Technically, we can support notification preferences independently of where the notifications are coming from. VA Profile supports preferences both for notifications supported by VANotify, and those that are supported by other VA systems. If and when we integrate notifications with VANotify depends on the health apartment roadmap and when features need to be fully supported on VA.gov.

**When and how will we integrate Cerner data?**

A huge piece of the entire apartment is integrating Cerner data, and notification preferences are no different. We will need to work closely with the health apartment team to figure out how to reconcile MHV and Cerner data for users who may go to one facility that uses Cerner and one that uses VistA. We hypothesize that it may be easier to integrate MHV data first, and then later figure out how to reconcile Cerner data.

**Do the VA.gov profile and the MyHealtheVet profile need to support the same notification preferences at the same time?**

Figuring out whether or not the VA.gov preferences can or should coexist with the MHV preferences affects how we approach things on the MHV end of things. If MHV wants our profiles or given preferences to coexist, they'll be in a position where they have to integrate with VA Profile. If not, we would want to make sure we had a coordinated approach where we turn off the MHV preference when we turn on the VA.gov preference.

## Problem Statement

- As a VA health care recipient, I want to choose how the VA communicates with me about difference aspects of my health care.

## User outcomes

### Desired User Outcomes

- Users can easily find and update their health care notification settings within the VA.gov profile, both before the health apartment is complete, and after.

### Undesired User Outcomes

- Users are confused about where to manage their health care settings while the MHV and VA.gov profiles coexist.
- Users have a difficult time signing in to VA.gov to change their notification settings before MHV is retired.

## Business outcomes

### Desired Business Outcomes

- VA.gov supports the existing MHV notification preferences, and some new ones, as part of this engagement.
- There is a clear path to guide users to the VA.gov profile once this functionality is supported on VA.gov.

### Undesired Business Outcomes

- (For VA.gov) We are put in a position to support a bunch of new settings that aren't actually ready to be supported.
- Users are confused about where to manage their health care settings while the MHV and VA.gov profiles coexist.

## Measuring success

OKRs and KPIs TBD.

## Solution approach

**Phase one: Definition, scoping, and planning - Fall 2022**

- We are engaging biweekly with the MHV team in order to define their notifications and notification preferences. This includes both existing notifications and notifications they are planning to add.
- Once we have a clear definition of what they have and what they would like to add, we will regroup with the health apartment team (eg. Lauren, Coulton, etc) to talk about a roadmap for these notifications & preferences. We hypothesize that we'll move over and incorporate notifications and preferences as related features (eg. secure messaging) are integrated into VA.gov.
- We will also talk to the health apartment about a migration strategy, and whether or not we think MHV should integrate with VA Profile, or we should simply retire notification preferences on MHV when we turn them on on VA.gov.

### Requirements

TBD

### Key dates

- February 2022: Begin MHV profile audit
- April 2022: Complete MHV profile audit findings report
- June 2022: Share audit findings with MHV team
- August 2022: Began MHV <> VA.gov biweekly meetings to scope out definition for notification preference migration in preparation for a VA Profile intake form

## Backend

## Frontend

## Design

### Previous research

- [Initial MHV profile discovery research findings](https://github.com/department-of-veterans-affairs/va.gov-team/tree/master/products/identity-personalization/profile/Research/2022-05-MHV-profile-research)

### Design artifacts

- Add link to use cases
- Add link to Sketch files

