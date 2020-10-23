# Points Eligibility, Tracking & Logistics

## General Guidelines
Follow these gardening guidelines to be eligible for [prizes](prizes.md) all month long, and set us up for maximum community impact. 
- All participants earn points, redeemable for [prizes](prizes.md), for each individual contribution made between 12 AM PDT October 19th through 9 AM PDT November 12th. 
- Review the list of [eligible contributions](project-ideas.md) to see what’s eligible&mdash;pull requests are most welcome, but explore other ways to add value.
- Attendees must [register for Summit Gardening Days](https://events.linuxfoundation.org/spinnaker-summit/register/) to be eligible to earn [prizes](prizes.md).
- Attendees must [check in](https://go.armory.io/gardener-checkin) to be eligible to earn [prizes](prizes.md) and appear on the [leaderboard](https://go.armory.io/contributors).
- Teams must demo their project at the demo session on November 12 at 9:00 AM Pacific, or add a demo post to [#gardening-general](https://spinnakerteam.slack.com/archives/CV4A90DPF) before 9:30 AM Pacific on November 12, to be eligible for a team prize package.
- Match advisors will use your answers to the registration questions to place you on a team. During kickoff week or after you've registered, we will notify you of your team placement to confirm participation, and provide Slack introductions to teammates. 
- Teams can mention @on-call-gardener and @gardening-admin in Slack for help in choosing a project.
- Read more about how to get started on the [getting started](getting-started.md) page

## Challenge Judging

Along with individual rewards, we will award team [prizes](prizes.md) using an anonymous judging process. We'll use Google Forms to create a demo survey, and will finalize it to include all eligible projects at or before 9:30 AM Pacific on November 12. During the demo session, our panel of on-call-gardeners, organizers, and SDLC partners will use the survey to vote for the winners.
We will award divisible team [prize packages](#prizes) to winning teams at the demo's conclusion and on Slack in [#gardening-general](https://spinnakerteam.slack.com/archives/CV4A90DPF).


## Points Tracking

Visit the [Leaderboard](https://go.armory.io/contributors) to track your points! Gardening organizers will track and tally points based on GitHub activity in eligible organizations, and other eligible content contributions as tracked in the [spinnaker-hackathon](https://github.com/spinnaker-hackathon) organization and in the [#gardening-general](https://spinnakerteam.slack.com/archives/CV4A90DPF) channel on [Spinnaker Slack](http://join.spinnaker.io).

### GitHub Event Contributions

To receive points for your open source GitHub contribution activity during Gardening, you must work in a tracked organization. These include:
- [Spinnaker](https://github.com/spinnaker)
- [Spinnaker-Hackathon](https://github.com/spinnaker-hackathon)

Eligible GitHub events include __pull request creation__, __commiting__, __issue creation__, and __issue and pull request commenting__ in Spinnaker project repositories.
Those event types, along with __pushing__ and __repository creation__ will be tallied where contributors can perform those events, in [spinnaker-hackathon](https://github.com/spinnaker-hackathon).

You should create repositories for the work in this [spinnaker-hackathon](https://github.com/spinnaker-hackathon) organization to receive GitHub event points for contributions such as:
- Demos
- Plugins
- Automation projects

All participants will be added to the [spinnaker-hackathon](https://github.com/spinnaker-hackathon) organization after checking in to the event. If you would like your work in another public repository
to be counted, mention @gardening-admin in [#gardening-general](https://spinnakerteam.slack.com/archives/CV4A90DPF), and we will evaluate exceptions on a case-by-case basis.

### Slack Tracking for Content Contributions 

To submit content for points eligibility, do the following:
1. If possible, initiate it in a respository in the [spinnaker-hackathon](https://github.com/spinnaker-hackathon) organization (see [Extra Points Opportunity](#extra-points-opportunity-for-content) below). 
2. Once content is published in its public destination, take a clear screenshot of it.
3. Post a message about your contribution in [#gardening-general](https://spinnakerteam.slack.com/archives/CV4A90DPF). Your message should include:
    - Screenshot
    - Your GitHub username
    - A brief description of the content  
4. After you post your message, add a :goldcoin: emoji reaction to your message. _Your points will not be counted unless you add this reaction_. If needed, [learn how to use reactions in Slack](https://slack.com/help/articles/206870317-Use-emoji-reactions). 

#### Extra Points Opportunity for Content

You have multiple opportunities to receive points for content contributions such as:
- Tutorials
- Blog posts
- Solution briefs
- Whitepapers
- Training guides
- Videos
- Twitch streams
- Contributor interviews

These contributions are eligible for points as [GitHub event contributions](#github-event-contributions) if you initiate the content or scripts 
as respositories in the [spinnaker-hackathon](https://github.com/spinnaker-hackathon) organization, and then __again__ as [Content contributions](#slack-tracking-for-content-contributions) once you post or publish them and follow the steps to redeem your points!

Besides those listed above, content contributions include community help responses, such as __stackoverflow answers__ and __spinnaker slack answers__. While these shouldn't be added to a repository and are not eligible as GitHub event contributions, they will earn points through the [Slack tracking system for content contributions](#slack-tracking-for-content-contributions). See a list of contribution types on the [What to Hack](https://spinnaker.io/community/gardening/what-to-hack/) page. 

## Leaderboard

Use our [Leaderboard](https://go.armory.io/contributors) to track your contribution totals, noting the time delay detailed below. We will use the following query against the [GH Archive dataset of public GitHub activity](https://www.gharchive.org/) to track contributions according to organization name:

```
SELECT
  actor.login,
  COUNT(*) as cnt,
FROM
  `githubarchive.month.*`
WHERE
  (repo.name LIKE 'spinnaker/%' OR  repo.name LIKE 'spinnaker-hackathon/%')
  AND created_at >= '2020-10-19 08:00:00'
  AND created_at < '2020-11-12 18:00:00'
  AND _TABLE_SUFFIX > '2020'
  AND type IN ('IssuesEvent',
    'IssueCommentEvent',
    'PullRequestReviewCommentEvent',
    'PullRequestEvent',
    'PushEvent',
    'CreateEvent',
    'CommitCommentEvent')
GROUP BY
  actor.login
ORDER BY cnt DESC
LIMIT
  180
```
Note: Our leaderboard on Google Sheets uses BigQuery to grab this data. This archive is a great way to get it, but there is a lag in the way the data is aggregated from GitHub APIs and aggregated into the archive. There is typically a 24-hour lag in the reflection of GitHub events in the archive, but it can sometimes be longer than 24 hours depending on what time the contribution was made. Therefore, __there will be a delay__ in the visualization of your contributions.





## The Spinnaker-Hackathon Organization

#### Create repositories
Starting fresh with some new plugin code, or writing a tutorial? Create all new project repositories in [Spinnaker-Hackathon](https://github.com/spinnaker-hackathon). Name your repo with a descriptive project string that you’ll use in your Slack channel name. Note: Your GitHub handle will be added as a member to the Spinnaker-Hackathon organization after registration, and you must register to receive repository creation privileges if this is your first Spinnaker Gardening Days.

#### Fork Spinnaker repositories
Need to fork an existing Spinnaker project(s) to hack? Fork into the [Spinnaker-Hackathon](https://github.com/spinnaker-hackathon):
![where to fork](/org-fork.png)
When it's time to submit a pull request, do so from your fork. Read more on [best practices in fork & pull request workflows](https://gist.github.com/Chaser324/ce0505fbed06b947d962).
