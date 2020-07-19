# Projects, Teams & Ideas @ Spinnaker Gardening Days

A list of Spinnaker project ideas organized into categories for your browsing pleasure. If you find an idea you're interested in and want to learn more, feel free to visit one of the associated team channels listed below, or post in [#gardening-general](https://spinnakerteam.slack.com/archives/CV4A90DPF)

## Amazon ECS
- [Adding capacity provider APIs or UI to Spinnaker](https://github.com/spinnaker/spinnaker/issues/5400#issuecomment-657258812)
  - Visit [#gardening-team-ecs](https://spinnakerteam.slack.com/archives/C017W527480) to seek collaborators and check progress
- [Adding a service metrics API/UI to Spinnaker](https://github.com/spinnaker/spinnaker/issues/5605#issuecomment-656920886)

## Spin CLI
- [Extending project functionality for the Spin CLI](https://trello.com/b/TZEErakm/extending-project-functionality-for-the-spin-cli)
  - Visit [#gardening-team-1111](https://spinnakerteam.slack.com/archives/C016P8K15AB) to seek collaborators and check progress

## Content Projects
- End-to-end SDLC from code commit to production using a combination of Jenkins + Spinnaker, including a canary deployment with metrics from Prometheus
  - Visit [#gardening-team-autobots](https://spinnakerteam.slack.com/archives/C016YHBQQLE) to seek collaborators and check progress
- Create a blog post or video about a Spinnaker webinar or conference talk:
  - 7/21 - The Culture Factor: Trust, Safety, and Continuous Delivery - Learn more about the combination of new technologies and new cultural behaviors that unlock accelerated innovation. Featuring Armory CTO Isaac Mosquera. [Register here](https://cd.foundation/webinars/).
  - 7/22 - Spinnaker @ DevOps Open Source Insights and Innovations - See a demo of the [new Splunk application for Spinnaker](https://splunkbase.splunk.com/app/5135/) from its creator, Chad Tripod. [Register here](https://events.splunk.com/OpenSource22072020?utm_campaign=Global_FY21Q2_Glbl_Armory_OnlineEvnt_AppDev_EN_VirtEvnt_PromoE_Jun20&utm_content=Open%20Source%20Insights).
  - Browse the [Spinnaker.Live Playlist](https://www.youtube.com/playlist?list=PL4yLrwUObNkvO80Bjln8_DJXxQNSYrtEs) for interesting talks to write about.

## Plugins
- [Add features to the [Nomad Plugin](https://github.com/hashicorp/nomad-spinnaker) to introduce custom stages into orca that support deployment of workloads to Nomad clusters
  - Visit [#gardening-team-autobots](https://spinnakerteam.slack.com/archives/C017JTAGGKB) to seek collaborators and check progress
- [Plugin to trigger pipelines on Azure blob storage artifacts](https://github.com/spinnaker/spinnaker/issues/3776)
  - Visit [#gardening-team-fresh](https://spinnakerteam.slack.com/archives/C017CF13A5A) to seek collaborators and check progress
- Plugin to automate extraction of key [DORA metrics](https://stelligent.com/2018/12/21/measuring-devops-success-with-four-key-metrics/) from Spinnaker pipelines
  - Visit [#gardening-team-grafana](https://spinnakerteam.slack.com/archives/C0180H97T9N) to seek collaborators and check progress
- [Plugin to add support for Microsoft Teams notifications to Echo](https://github.com/spinnaker/spinnaker/issues/5826)
  - Visit [#gardening-team-ms-teams-notifications](https://spinnakerteam.slack.com/archives/C0174Q285L6) to seek collaborators and check progress
- Stage plugin for enabling manual judgements that require data entry 
  - Sometimes approvers for production changes need to manually input information as part of a manual judgement, such as documentation links or further explanation. This plugin could replace or augment the standard manual judgment approval dropdown with a text field in Deck.
  - Ping @AbdulBasit in [#gardening-general](https://spinnakerteam.slack.com/archives/CV4A90DPF) for context

## Other Integrations
These may or may not be implementable as plugins
- [Integrate Kafka as a Pub/Sub system in Echo](https://github.com/spinnaker/spinnaker/issues/2117)
  - Visit [#gardening-team-crickets](https://spinnakerteam.slack.com/archives/C017489TB8B) to seek collaborators and check progress
- [Add support for AWS CloudWatch metrics in Kayenta](https://github.com/spinnaker/spinnaker/issues/5888)
  - Visit [#gardening-team-crickets](https://spinnakerteam.slack.com/archives/C017489TB8B) to seek collaborators and check progress

## Bugfixes & Service Improvements
- [Fix invalid YAML deletion from Manifest Source field upon save](https://github.com/spinnaker/spinnaker/issues/5357)
  - Visit [#gardening-team-issue-5357](https://spinnakerteam.slack.com/archives/C011ALS3F41) to seek collaborators and check progress
- Add ingress URLs to the Infrastructure tab
  - Service URLs are shown in the load balancers area, but not ingress URLs. It would be really useful for end users to have the ingress right there to access the deployed app if needed, since many web apps don't use the load balancer URL, but the ingress instead.
  - Ping @AbdulBasit in [#gardening-general](https://spinnakerteam.slack.com/archives/CV4A90DPF) for context



