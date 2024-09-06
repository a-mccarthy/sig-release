# Kubernetes Release Team: Communications Coordinator

## Overview

The Communications Coordinator role is responsible for facilitating, empowering, and curating communication between the release team and various stakeholders including the Cloud Native Computing Foundation (CNCF), the media, contributing vendors, Kubernetes project managers, and the overall Kubernetes community at large.

Communications deliverables that come from the release process include a release blog, an optional removals and deprecations blog, facilitation of a feature blog series, scheduling of a CNCF Kubernetes release webinar as well as other speaking opportunities, and approved messaging for media. In the event the release schedule slips, the communications coordinator will ensure media opportunities through the CNCF are synchronized and that all stakeholders are kept advised of changes in timing.

## Requirements

**Before continuing on to the Communications specific requirements listed below, please review and work through the tasks in the [Release Team Onboarding Guide](/release-team/release-team-onboarding.md).**

### Skills and Experience Required

- Strong written and verbal communications skills
- A working knowledge of Kubernetes concepts
- Fundamental GitHub skills and experience with open source projects
- Enough experience with the Kubernetes release process to understand how communications milestones fit into the overall release
- Project management experience
- Existing relationships with the CNCF, relevant media personnel and outlets, Kubernetes project managers, and vendor stakeholders is helpful, but not required
- The communications lead should take the [Inclusive Speaker Orientation (LFC101)](https://training.linuxfoundation.org/training/inclusive-speaker-orientation/) training course

### Expected Time Investment

The Kubernetes release cycle spans 15 weeks, however it may run longer. The typical workload for the communications team is very light during the first few weeks of the release cycle. In the later weeks, **the workload can become heavy, and will continue a few weeks after the release.**

The expected time investment for both leads and shadows are as follows:

- 30 minutes to 2 hours a day (depending upon week), requesting and reviewing incoming KEPs and blog PRs, working with other SIGs or the CNCF to manage the feature blog posts, and following Slack channels in order to keep pending content current.

- 1 to 5 hours a week, attending
    - Release Team (weekly) 
    - SIG Docs Team (biweekly) and 
    - Burndown meetings (daily during Code Freeze).

**NOTE:** These are estimates and your personal experience may vary. The keys to success in this role are collaboration with the team and maintaining regular communication within the team.

## External Release Communication

Please use the `release-comms@kubernetes.io` Google Group list for external release communications (communicating with the CNCF, etc.).

The following groups should be members:
* The current release cycle's Release Team Lead & Lead Shadows
* The current release cycle's Communications Lead & Comms Shadows
* SIG Release Chairs

The list must rotated/actively managed every cycle. Submit a PR to update [this document](https://git.k8s.io/k8s.io/groups/groups.yaml) per the milestone activities described below.

### Slack Channel

There is a channel on the Kubernetes Slack workspace, `#release-comms`, which is used by the communications release team to coordinate their efforts. If you're on the communications team, or applying to be, then it would be advantageous to follow along with the conversations. The Communications Coordinator (often referred to as the "Comms Lead") should post a status here at a regular cadence to keep release team members and other stakeholders informed.

How a particular team communicates day-to-day is up to the Comms Lead and teams members, but usually they Slack DM on day-to-day coordination and post summary updates in `#release-comms`.  

## Release deliverables

Throughout the release cycle, the main Communications deliverables include:
* **Collection of Release Highlights.** The Communications team coordinates with SIG Leads to solicit Release Highlights for the release, to be used in both the Release Blog and Release Notes.
* **Authoring the Kubernetes release blog.** The Communications team writes the release blog, which is the official announcement of the Kubernetes release. This includes the Release Highlights from SIG leads.
* **Coordination and support of the feature blog series.** SIGs opt-in to author feature blogs for the release. These blogs are written by technical owners, and the Communications team supports authors from the early stages through facilitating editorial and tech reviews as well as publication.
* **Coordination and support of an optional Deprecations and Removals blog.** Depending upon the content of a given release, it may be necessary to prepare the community for upcoming deprecations and removals. This is decided per release cycle around the time of Code Freeze.
* **Scheduling press activities and the post-release webinar with the CNCF.** The Communications Coordinator works with the CNCF to schedule press release activities around the release, and to schedule the release webinar (typically scheduled 3-4 weeks post-release).

### Collect Release Highlights

A GitHub Discussion must be open to invite all SIG leads and members to add Release Highlights for inclusion in the Release Blog and Release Notes. The discussion must be opened in kubernetes/sig-release under General Category. 

Past discussions: [1.25](https://github.com/kubernetes/sig-release/pull/1987), [1.24](https://github.com/kubernetes/sig-release/discussions/1868), [1.23](https://github.com/kubernetes/sig-release/discussions/1709), [1.22](https://github.com/kubernetes/sig-release/discussions/1575), [1.21](https://github.com/kubernetes/sig-release/discussions/1436).

Each SIG should be pinged via their individual Slack channels and the #chairs-and-techleads channel to solicit suggestions, and each KEP owner should be asked about inclusion as a Release Highlight at the same time Feature Blogs are being solicited.

The Communications team should hold a meeting to discuss Release Highlights sometime around Code Freeze. Ensure that at least one person from the Release Notes team attends this meeting with the Release Lead and Enhancements Lead.

### Release blog

The Communications Coordinator along with the Comms shadows are responsible for authoring the official Kubernetes Release blog. This blog is the official statement of release. The release blog is the primary vehicle by which the release team communicates the release highlights, known issues, and other aspects of the release to the community. 

Start the draft with the team around week 12, striking a balance between the enhancements being close to finalized and having enough to time author the blog and have it reviewed. Ahead of review, open a pull request on the [website repository](https://github.com/kubernetes/website) and assign the release lead and other stakeholders as reviewers.

It's up to you and your team regarding how best to do this. Typically it works well to assign sections to different team members (e.g. Release Highlights, User Highlights, Ecosystem Updates, etc.) and have the lead pull it all together and manage the PR and reviews.

The release lead will drive the content for the release theme and logo. 

### Feature blogs

Tracking, facilitating, and organizing the publication of the Feature Blog series is a major deliverable of the Comms team. Feature blogs are opt-in for SIGs, and are authored by enhancement developers and others close to the features. We do, however, need to encourage owners of important enhancements to opt in to writing feature blogs. 

Examples of enhancements that warrant a feature blog might include: 
* breaking changes 
* features and changes important to our users 
* features that have been in progress for a long time and are graduating 
* features that are considered mandatory by the Release Lead.

It helps to work closely with the Release Lead and use the respective SIG Slack channels to remind the SIGs about opting in to feature blogs and provide any necessary context to blog authors. 

**Reach out in KEP issues to ask for feature blog opt-in.** Ask every KEP owner if they want to contribute a blog by reaching out in the KEP issue. Example messaging is below.

```
👋 from the v1.31 Communications Team!
We'd love for you to consider writing a feature blog about your enhancement! Some reasons why you might want to write a blog for this feature include (but are not limited to) if this introduces breaking changes, is important to our users, or has been in progress for a long time and is graduating.  

To opt-in, let us know and open a Feature Blog placeholder PR against the [website repository](https://github.com/kubernetes/website) by **[BLOG PLACEHOLDER PR DEADLINE]**. For more information about writing a blog see the [blog contribution guidelines](https://kubernetes.io/docs/contribute/new-content/blogs-case-studies/#technical-considerations-for-submitting-a-blog-post).

Note: In your placeholder PR, use `XX` characters for the blog `date` in the front matter and file name. We will work with you on updating the PR with the publication date once we have a final number of feature blogs for this release.
```

NOT EVERY KEP NEEDS A BLOG. Work with the KEP owners, Release Lead, and SIG Docs Blog team (though #sig-dcos-blog slack channel) to make sure all KEPs that opt-in really need a blog written. If a feature is small, or new in Alpha it may not be ready for a blog. 

**As feature blogs are opted in and placeholder PRs are created**, assign the blogs to shadows and yourself for tracking and facilitation. The Comms team is responsible for making sure blog authors have the resources and information they need to write the blog, and tracking the blogs progress through editorial and tech reviews once the blog is ready. 

> Some features that opt-in to writing a blog may miss the code freeze deadline. Blog placeholder PRs for features that are no longer in the release should be closed.  

When a placeholder PR is created, make sure the PR has been held using the `/hold` command. Feature blogs should not be merged **until after the release date and the comms team has assigned a publication date**. 

Anyone can hold a PR by adding a comment with the `/hold` command, like the example below. This will to apply the `do-not-merge/hold` label to the PR and will prevents the PR from merging until the label is removed. This will stop a blog from accidently merging and publishing ahead of the release. [1.31 Example](https://github.com/kubernetes/website/pull/46911#issuecomment-2185024105).

```
/hold

Pending assignment of publication date by release comms. This blog should be held until the vX.XX release has happened.
```

Once the release has happened, use the `/unhold` command to remove the `do-not-merge/hold`. 

#### Creating a blog publication schedule

**The Comms team establishes the feature blog publication schedule.** Other members of the release team or blog reviewers may contribute ideas and feedback on the schedule, but ultimately the schedule is determined by the Comms team. 

Use the blog schedule field in the Feature Blog view on the tracking board to assign a publication date.

Feature blog publication usually starts the day after the release. The release blog goes out on same day as the release and the first feature blog typically goes out the day after the release. The rest of the blogs are published one-at-a-time, typically at a rate of two to three posts weekly. Depending on how many feature blogs you have, you may want to publish one per day after the release. In general, all feature blogs should be published within month of the release day.

> Note that blog PRs in k/website are dated, and automation will publish future-dated entries. This enables a PR process decoupled from blog publication date. Once a blog has passed the review process it can be merged and will be published on the date on the blog. 

**Communicate the planned publish date to SIG Docs and the owner of the feature blog**. Notify the author in the PR and Slack channels: `#sig-docs-blog`, `#sig-docs` about the schedule. The communications team will assist in coordinating and publishing the feature blogs on schedule.
> See example [here](https://github.com/kubernetes/website/pull/41924), "this article is scheduled for the 21th of August".

Please note that the release team will support the blog publication after the release day too. 

#### Feature blog reviews

Also see the docs for [pull requests review process](https://kubernetes.io/docs/contribute/review/reviewing-prs/) and [reviewing a pull request](https://kubernetes.io/docs/contribute/review/for-approvers/#reviewing-a-pr).

**Work closely with the [SIG Docs Blogs](https://github.com/kubernetes/community/tree/master/sig-docs/blog-subproject) team.** These are the folks responsible for editorial reviews (and sometimes tech reviews) of Kubernetes blogs. The Comms lead should plan to regulary share updates on blog status and review timelines with the blog reviewers via `#sig-docs-blogs` and during sig-docs meetings. 

Each blog should pass 2 "official" reviews, an editorial review and tech review. Anyone is open to do an "informal" review on any blog and leave suggestions. As part of the comms team, it's encouraged (but not required) to help reviews blogs for both editorial and technical correctness if you have time. 

An official review comes from someone with [permission to add the lgtm label](https://kubernetes.io/docs/contribute/review/for-approvers/#prow-commands-for-reviewing) to a pull request.
* **Tech reviews** usually come from the sponsoring SIG. If you dont see a tech review on the blog, reach out to the author to make sure the PR has been flagged for review. You can also reach out in the SIG slack channel to ask for help with tech reviews. 
* **Editorial reveiws** usually come from blog reviewers or SIG Docs reviewer. They make sure that the blog is readable and adheres to the [style guide](https://kubernetes.io/docs/contribute/style/style-guide/).

Once a blog has the `lgtm` label assigned an [approver] can add the `aprove` label to get the PR merged. Note that reviews can still happen on blogs with a `lgtm` label 
 

## Working with other teams and SIGs

Throughout the release cycle the comms team works with lots of different teams within the Kubernetes community. As a Comms lead or member of the comms team, you should feel empowered to reach out and ask questions or as for help from SIGs and other Release team members to meet deadlines.

Some groups you may need to contact include

* SIG Contributor Experience in the `#sig-contribex`slack channel and by attending meetings. They can help promote the feature blogs through social media.
* Chairs and Tech Leads of SIGs in the `#chairs-and-techleads` slcak channel. This can be a helpful place to post reminders about blog deadlines SIG leads to see.

### Mid-cycle deprecations and removals blog

This blog is optional and will vary from release to release. Work with the rest of the release team ahead of **the Code Freeze date to determine if a mid-cycle blog focused on feature deprecations and removals is warranted**.

If so, facilitate its creation and publication. You can create a Slack thread on [#sig-release](https://kubernetes.slack.com/archives/C2C40FMNF) and `#sig-docs-blog` to discuss this.

If the release will deprecate important and commonly-used features (or simply a large number of features will be deprecated), consider publishing this blog. 

Also consider this when commonly-used features that have been deprecated are removed in a release. Follow these examples:
- [Kubernetes API and Feature Removals in 1.22](https://kubernetes.io/blog/2021/07/14/upcoming-changes-in-kubernetes-1-22/)
- [Deprecated APIs Removed in 1.16](https://kubernetes.io/blog/2019/07/18/api-deprecations-in-1-16/)
- [Kubernetes Removals and Major Changes In 1.25](https://kubernetes.io/blog/2022/08/04/upcoming-changes-in-kubernetes-1-25/)

> Publication should occur ahead of the release in order to inform the community and allow for preparation time. Start the discussion mid-cycle and well ahead of Code Freeze, and target publication for Code Freeze week.

### Press and release webinar

This is a simple but very important component of the Communications Coordinator role. Two sets of activities need to be scheduled with the CNCF:
- press release and interview scheduling around the release day and
- the release webinar after the release.

You will be a liaison between the Release lead and the CNCF contacts to schedule the press briefings. Send an email to `pr@cncf.io` about a month ahead of the release and coordinate between the parties to get release day press events scheduled.

See the sample email for schedule press and pre-briefings for the release lead with CNCF by emailing pr@cncf.io

```
CC'd release-comms and the release lead.
Title: Schedule interview for the release lead

Hi there,

I'm the comms lead for Kubernetes v1.xx (currently scheduled to release Tuesday 5th December 20xx), and I'm reaching out to get our release day and pre-release press handled. 

Thanks,
Communication Team 1.xx
```

To schedule the release webinar with the CNCF, start things with an email to `webinars@cncf.io`. You will likely use the Calendly link (below) to schedule a "live webinar". If things are tight on the schedule, CNCF will help find a spot.

The webinar is typically scheduled for 3-4 weeks after the release and is primarily presented by the Release lead and Enhancements lead. Often the Comms lead will also join the webinar. The format is open, but primarily the team walks through the enhancements in the release and gives a sneak peek of what's coming in the next release.

See the sample webinar email below for reference.

```
title: Scheduling the Kubernetes 1.xx Release Live Webinar

Hi there! I'm the communication lead for Kubernetes v1.xx, XXXX, and I'm reaching out to schedule a live webinar for our release and enhancements leads. Could you help us to schedule in the Calendly: https://calendly.com/cncfonlineprograms/livewebinar

This version is currently scheduled to land Tuesday 5th December 20xx, see the details here: https://www.kubernetes.dev/resources/release/ 

Do you have availability sometime for 3-4 weeks after the release, maybe between x-x in December?

Thanks,
Comms Team 1.xx
```

Refer to the [slides](https://docs.google.com/presentation/d/10y65ptwXQrt_0P6sA3TSvRH_c7TGBc8DEHhXRNwi-10/) and [webinar](https://www.youtube.com/watch?v=BTPlVsgO_As) from the 1.22 release as an example.

Note you'll need to send headshots and company/title information when you schedule the webinar and the slides should be sent for CNCF review at least one week ahead of the webinar.


### Social posts

The Release Communications team is **NOT** responsible for social posting. [SIG Contributor Experience](https://github.com/kubernetes/community/tree/master/sig-contributor-experience) (SIG Contribex) manages the official Kubernetes social accounts and is responsible for all posts to those accounts. SIG Contribex has created automation around blog posts, so once a blog is published to the Kubernetes website, social posts are created and posted according to their automation schedule. 

If the Communications team and Release Lead determine a feature or other release communication needs a more detailed communications or calls to action, reach out to with SIG Contributor Experience for help making posts use the `@contributor-comms` tag in the `#sig-contribex` Slack channel. 

### Tips and best practices

#### Use the 2 week rule

Try to give 2 weeks notice for all deadlines and requests for reviews. When planning to reach out for blog opt-in or asking for reviews on blog drafts, you should start posting messages or have blog drafts ready for review at least two weeks from the deadline. Especially when asking for blog reviews, as the blog team is understaffed, this will give reviewers enough time to do the review and you enough time to address any feedback. This is best effort, as the schedule does not always allow for this much lead time before a deadline.

#### Reaching out to KEP owners, blog authors, and reviewers

Post messages to GitHub or in SIG slack channels for the best visibility into ongoing work and to allow other contributors to help. Having messages in the KEPs, blog PRs, or SIG slack channels, can help centralize information about the work being done and any outstanding issues. If you need to escalate an issues to Release Leads or SIG Chairs, having public messages/records of conversations can make it easy to tag who you need to. 

If you do use direct messages to contact someone during a release,  if you have been unable to get ahold of them through other public channels for example, post summaries of the conversation to PRs or SIG slack channels. This way everyone can stay up-to-date on the ongoing work.

#### Deadlines

As much as possible stick to the comms deadlines set in the release schedule for the mid-cycle blog and main release blog. This will ensure that no release-blocking issues come up and that these blogs go out when they need to.

Feature blog deadlines are a little more flexible compared to other release deadlines. Because the feature blogs are published after the release, there is usually more time to review them if a deadline is missed. In general, as long as blog authors are responsive and blog content is getting added/reviewed, its OK to give authors extra time to finish their work. If you feel that a blog author is not responsive, progress has not been made, and the dealines have been stretched too far, escalate to the release or SIG chairs or cancel the blog. A blog can always been written outside of the release cycle. 

## Release Milestone Activities

This is an example of a typical release cycle and the order of how tasks will flow for Comms. Note that some tasks may take longer than their designated "release week". Each release is a little different, the following guideline is only a suggestion. You should always refer to the specific release schedule for exact dates and deadlines in a release cycle. 

<table>
    <tr>
        <td><h3><b>Release Week</h3></b></td>
        <td><h3><b>Milestones</h3></b></td>
        <td><h3><b>Activities</h3></b></td>
    </tr>
    <tr>
        <td>1</td>
        <td><b>Start of release cycle</b></td>
        <td>
        <ul>
        <li>Start attending the Release Team weekly meeting
        <li>Join the following Slack channels: <code>#sig-release</code>, <code>#release-comms</code>, <code>#sig-docs</code>, and <code>#sig-docs-blog</code>.
        <li>Check if there are any holidays or events (e.g. KubeCon) that will occur during this release which may impact communication with the CNCF and SIG Chairs, plan accordingly
        <li>Select shadows for the team
        <li>Ensure shadows are all in the Kubernetes org on GitHub
        <li>Ensure you and your shadows are entered into the release contact sheet
        <li>Ensure you and your shadows are on the release team meeting invites
        <li>Establish initial meeting with the Comms team to introduce everyone and review tasks and the release timeline
        <li>Plan a regular-cadence Comms team sync up (mostly needed toward the end of the cycle)
        </ul>
        </ul>
        </td>
    </tr>
    <tr>
        <td>2</td>
        <td></td>
        <td>
        <ul>
        <li>Update the <code>release-comms</code> Group. <a href="https://github.com/kubernetes/k8s.io/blob/main/groups/sig-release/groups.yaml">Membership</a> for this group is defined in <a href="https://git.k8s.io/k8s.io">kubernetes/k8s.io</a>. Ensure the list <b>only includes</b>:
        <ul>
        <li>The current release cycle's Release Team Lead & Lead Shadows
        <li>The current release cycle's Communications Lead & Comms Shadows
        <li>SIG Release Chairs 
        </ul></ul>
        <ul>
        <li>Start communications with the SIG leads to align on the communications timeline and support for writing feature posts
        <li>Setup a communications plan aligned with the Release Calendar
        <li>Agree on participation together with Enhancements team lead at the next SIG Leads monthly meeting to align on expectations and communication possibilities
        </ul>
        </td>
    </tr>
    <tr>
        <td>3</td>
        <td><b>Production Readiness Freeze</b></td>
        <td>
        <ul>
        <li>Get access to the <code>Enhancements</code> and <code>Feature blog opt-in</code> tracking boards and start following along. Edit the <code>Comms Opt-in Assignee</code> and <code>Comms Editor</code> columns with everyone on the comms team.
        </ul>
        </td>
    </tr>
    <tr>
        <td>4</td>
        <td><b>Enhancements Freeze</b></td>
        <td>
        <ul>
        <li>Work with the enhancements lead to understand big-ticket items to be included in the release
        <li>Start monitoring the <code>Feature blog opt-in</code> sheet for new entries and use the <code>Assigment tab</code> sheet to assign and track status throughout the cycle (<a href="https://docs.google.com/spreadsheets/d/1hgFWig6YBSYORP3huwEyU0VlXGcYi6wMxjYW-swzCIY">for example</a>)
        <li> With Enhancement freeze in effect, create a GitHub discussion (<a href="https://github.com/kubernetes/sig-release/discussions/2047">example v1.26</a>) to start collecting the Release Highlights of the release, and reach out to all SIGs on and off over the next few weeks to ask for Release Highlights and explain why this is important to the community.
        <ul>
        </ul>
        </ul>
        </td>
    </tr>
    <tr>
        <td>5</td>
        <td></td>
        <td>
        <ul>
        <li>Work with Enhancements and Release Note leads to determine which deliverables are most noteworthy post-Enhancements Freeze
        <li>In the coming weeks, follow the progress of these enhancements, as they will roll into the Release Highlights and be called out and described in the release blog
        <li>Work with the Release Team and decide if the release warrants a mid-cycle 'Deprecations and Removals' blog. Generally, this is decided at a minimum of two deprecations or removals, or if there are significant deprecations and removals that will impact the community. 
        <li>If needed, solicit author(s) for a 'Deprecations and Removals' blog and get a placeholder PR in k/website for tracking
        </ul>
        </td>
    </tr>
    <tr>
        <td>8</td>
        <td></td>
        <td>
        <ul>
        <li>Post reminders for the feature blog opt-in on the SIG slack channels (<a href="https://kubernetes.slack.com/archives/C0BP8PW9G/p1622556913118800">for example</a>)
        <li>Assign feature blog topics as they come in to team shadows for support and tracking efforts
        <li>Join the <code>#sig-docs-blog</code> channel on Slack. Share the current status of the Feature blog opt-in's and in Slack and in the sig-docs call and work with the team to establish review expectations and publication strategy.
        </ul>
        </td>
    </tr>
    <tr>
        <td>10</td>
        <td></td>
        <td>
        <ul>
        <li>Send out final reminders for feature blog opt-in on the SIG slack channels or KEP issues
        <li>Facilitate or start writing the optional Deprecations and Removals blog
        <li>Coordinate with Release Notes to ensure Release Highlights are checked in before Code Freeze.
        </ul>
        </td>
    </tr>
    <tr>
        <td>11</td>
        <td><b>Feature blog freeze</b></td>
        <td>
        <ul>
        <li>Start attending burndown meetings
        <li>Participate in the release retro part 1
        <li>Feature blog freeze is this week
        <li>Assign remaining feature blog topics
        <li>Establish feature blog post-release publication schedule, typically 2-3 posts per week.
        <li>Post the feature blog publication schedule in <code>#sig-docs-blog</code> (<a href="https://kubernetes.slack.com/archives/CJDHVD54J/p1628649661040600">example post</a>)
        <li>Establish a regular cadence status check-in with the <code>#sig-docs-blog</code> team and maintain the publication schedule post in Slack to keep everyone synced
        <li>Request placeholder PRs in k/website from all feature blog authors
        </ul>
        </td>
    </tr>
    <tr>
        <td>12</td>
        <td><b>Code Freeze</b></td>
        <td>
        <ul>
        <li>Begin the release blog draft, if not yet started
        <li>Host a meeting with the Release Lead, Enhancements Lead, and Release Notes to discuss the Release Highlights to be highlighted in the release blog and ensure consistency with Release Notes
        <li>Optional 'Deprecations and Removals' blog ready for review
        <li>Schedule the release Live Webinar with CNCF by emailing <code>webinars@cncf.io</code>. You may be referred to <a href="https://calendly.com/cncfonlineprograms">Calendly</a>. The webinar is typically scheduled for 3-4 weeks after the release
        <li>Schedule press and analyst pre-briefings and interviews for the release lead with CNCF by emailing <code>pr@cncf.io</code>
        <li>Schedule release blog and press embargo with CNCF
        </ul>
        </td>
    </tr>
    <tr>
        <td>13</td>
        <td></td>
        <td>
        <ul>
        <li>Finalize and publish the 'Deprecations and Removals' blog once code freeze is in place.
        <li>Update release blog draft, post-Code Freeze
        <li>Check status with Release Notes lead on content for the Known Issues section of the release blog
        <li>Check status on all feature blog PRs. Keep <code>#sig-docs-blog</code> up-to-date for editorial review, and establish tech reviewers are available 
        </ul>
        </td>
    </tr>
    <tr>
        <td>14</td>
        <td><b>Feature Blogs ready to review</b></td>
        <td>
        <ul>
        <li>Feature blog reviews start
        <li>Continue to partner with <code>#sig-docs-blog</code> for editorial review, work to ensure tech reviews are moving forward from SIGs
        <li>Connect with Release Lead to ensure theme and release logo will be ready for release blog (not required for draft revisions)
        <li>Ensure that short one-to-two paragraph summaries of each Release Highlights are available for the release blog from Release Notes lead or SIG Chairs
        <li>Finalize Release blog final draft and start reviews
        <li>Send release blog draft to CNCF
        </ul>
        </td>
    </tr>
    <tr>
        <td>15</td>
        <td><b>Release Week</b></td>
        <td>
        <ul>
        <li>Finalize Release Blog, ensure it's ready for Docs Lead to publish on release day
        <li>Ensure first few feature blogs are ready to publish and that review and merge plans are in place for any still outstanding.
        </ul>
        </td>
    </tr>
    <tr>
        <td>16</td>
        <td><b>Release retrospective</b></td>
        <td>
        <ul>
        <li>Continue to facilitate publication of remaining feature blogs
        <li>Participate in release retro parts 2 and 3 (as needed)
        <li>Organize the slides for the CNCF release webinar, and send to the CNCF for review at least one week ahead of the scheduled date.
        <li>Update this document!
        </ul>
        </td>
    </tr>
</table>

## Release Blog Outline & Template
To support you in the creation of the release blog this [outline](/release-team/role-handbooks/communications/release-blog.md) summarize ideas for sections and gives you a template for easier release blog creation.
