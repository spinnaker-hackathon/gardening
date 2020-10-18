# Projects, Ideas, and Teams @ Spinnaker Gardening Days

A list of Spinnaker project ideas organized into categories for your browsing pleasure. If you find an idea you're interested in and want to learn more, feel free to visit one of the associated team channels listed below, or post in [#gardening-general](https://spinnakerteam.slack.com/archives/CV4A90DPF)

## Amazon ECS
- [Adding capacity provider APIs or UI to Spinnaker](https://github.com/spinnaker/spinnaker/issues/5400#issuecomment-657258812)
  - Visit [#gardening-team-ecs](https://spinnakerteam.slack.com/archives/C017W527480) to seek collaborators and check progress
- [Adding a service metrics API/UI to Spinnaker](https://github.com/spinnaker/spinnaker/issues/5605#issuecomment-656920886)

## Spin CLI
- [Extending project functionality for the Spin CLI](https://trello.com/b/TZEErakm/extending-project-functionality-for-the-spin-cli)

## GitHub and Actions Extensibility
- [Add support for GitHub Actions CI integration](https://github.com/spinnaker-hackathon/github-actions)

## Sumo Logic Extensibility
- [Expand the Spinnaker App for Sumo Logic](https://github.com/spinnaker-hackathon/sumo-logic/blob/main/README.md) to provide automated software delivery performance insights based on Spinnaker deployment acticity

## Content Projects
- Create and record a Spinnaker Twitch stream that live-demonstrates a small process or workflow
  - [Here's an example from the Tekton community](https://www.youtube.com/watch?v=LTRE8a22tio)
  - Spinnaker Twitch content should be posted to the Continuous Delivery Foundation account for maxiumum exposure
- End-to-end SDLC from code commit to production using a combination of Jenkins + Spinnaker, including a canary deployment with metrics from Prometheus
- Write a post about Spinnaker or a Spinnaker contributor for the [community blog](https://blog.spinnaker.io/). Need help finding someone to interview? Need help submitting your post to the blog? Mention @gardening-admin in [#gardening-general](https://spinnakerteam.slack.com/archives/CV4A90DPF).
- Create a blog post or video about a Spinnaker talk.
  - Find interesting talks on this year's [Spinnaker Summit schedule](https://events.linuxfoundation.org/spinnaker-summit/program/schedule/).
  - Browse the [Spinnaker.Live Playlist](https://www.youtube.com/playlist?list=PL4yLrwUObNkvO80Bjln8_DJXxQNSYrtEs) for interesting talks to write about.

## Plugins
- Add features to the [Nomad Plugin](https://github.com/hashicorp/nomad-spinnaker) to introduce custom stages into orca that support deployment of workloads to Nomad clusters
- [Plugin to trigger pipelines on Azure blob storage artifacts](https://github.com/spinnaker/spinnaker/issues/3776)
- Plugin to automate extraction of key [DORA metrics](https://stelligent.com/2018/12/21/measuring-devops-success-with-four-key-metrics/) from Spinnaker pipelines
- Stage plugin for enabling manual judgements that require data entry 
  - Sometimes approvers for production changes need to manually input information as part of a manual judgement, such as documentation links or further explanation.   - This plugin could replace or augment the standard manual judgment approval dropdown with a text field in Deck. Ping @AbdulBasit in [#gardening-general](https://spinnakerteam.slack.com/archives/CV4A90DPF) for context

## Other Integrations
These may or may not be implementable as plugins
- [Integrate Kafka as a Pub/Sub system in Echo](https://github.com/spinnaker/spinnaker/issues/2117)
- [Add support for AWS CloudWatch metrics in Kayenta](https://github.com/spinnaker/spinnaker/issues/5888)
- [Add support for AppDynamics metrics in Kayenta](https://github.com/spinnaker/kayenta/issues/770)

## Bugfixes
Don't forget to check the list of [beginner-friendly issues](https://github.com/spinnaker/spinnaker/issues?q=is%3Aopen+is%3Aissue+label%3A%22beginner+friendly%22) for good bugfixes to start with
- [Fix invalid YAML deletion from Manifest Source field upon save](https://github.com/spinnaker/spinnaker/issues/5357)

## Service Improvements
- Add ingress URLs to the Infrastructure tab
  - Service URLs are shown in the load balancers area, but not ingress URLs. It would be really useful for end users to have the ingress right there to access the deployed app if needed, since many web apps don't use the load balancer URL, but the ingress instead.
  - Ping @AbdulBasit in [#gardening-general](https://spinnakerteam.slack.com/archives/CV4A90DPF) for context
- Create a Helm templating library for generating Spinnaker pipeline templates
  - Ping @Suhrud in [#gardening-general](https://spinnakerteam.slack.com/archives/CV4A90DPF) for context and design details
- Create a "official" candidate Helm chart for installing Spinnaker that uses the Operator (instead of Halyard)
  - Default files (Note: NOT an implementation) have been added to Armory's open source [spinnaker-operator](https://github.com/armory/spinnaker-operator/tree/master/deploy/operator/helm) repo, and Armory is seeking contributions in this area
  
## Frontend UI/UX
Visit [#sig-ui](https://spinnakerteam.slack.com/archives/CH3FMKA3U) to seek collaborators and discuss ongoing UI/UX projects 

- Many buttons need tool tips, especially when the window is so narrow that buttons are shrunk to just icons with no visible label.
- Display why the Create button is grayed out in the new application form, so users know what they need to add or fix.
- Darken the add stage button color, so it looks less gray, (it may be guided by a style guide, or maybe a CSS value).

## Contributor Experience
- Create a visualization of a map of the world with the number of Spinnaker contributors from different countries
- Create a contribution tracking app more personal than DevStats. The app could show basic stats as associated with GitHub usernames (similar to devstats), but also include a login experience that allows users to access a more full-featured version of the app, in which they can "claim" the contributor profile attached to their GitHub account, add their name and link it to their linked-in profile, and show off all their contributions to CDF projects (Jenkins, Tekton, Screwdriver, and Spinnaker). Lots of different ways to get data from GitHub!
  - Visit [#contributor-game-app](https://spinnakerteam.slack.com/archives/C019EV8HA7Q) to collaborate on a Contributor Experience App for Spinnaker and the CDF. Check out our [work in progress](https://github.com/ExitoLab/spinnaker_gamification_app).




