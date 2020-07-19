A list of project ideas organized into categories

## Amazon ECS
- [Adding capacity provider APIs or UI to Spinnaker](https://github.com/spinnaker/spinnaker/issues/5400#issuecomment-657258812)
- [Adding a service metrics API/UI to Spinnaker](https://github.com/spinnaker/spinnaker/issues/5605#issuecomment-656920886)

## Spin CLI
- [Extending project functionality for the Spin CLI](https://trello.com/b/TZEErakm/extending-project-functionality-for-the-spin-cli)

## Content Projects
- End-to-end SDLC from code commit to production using a combination of Jenkins + Spinnaker, including a canary deployment with metrics from Prometheus
- Create a blog post or video about a Spinnaker webinar or conference talk:
  - 7/21 - The Culture Factor: Trust, Safety, and Continuous Delivery - Learn more about the combination of new technologies and new cultural behaviors that unlock accelerated innovation. Featuring Armory CTO Isaac Mosquera. [Register here](https://cd.foundation/webinars/).
  - 7/22 - Spinnaker @ DevOps Open Source Insights and Innovations - See a demo of the [new Splunk application for Spinnaker](https://splunkbase.splunk.com/app/5135/) from its creator, Chad Tripod. [Register here](https://events.splunk.com/OpenSource22072020?utm_campaign=Global_FY21Q2_Glbl_Armory_OnlineEvnt_AppDev_EN_VirtEvnt_PromoE_Jun20&utm_content=Open%20Source%20Insights).
  - Browse the [Spinnaker.Live Playlist](https://www.youtube.com/playlist?list=PL4yLrwUObNkvO80Bjln8_DJXxQNSYrtEs) for interesting talks to write about.

## Plugins
- [Add features to the [Nomad Plugin](https://github.com/hashicorp/nomad-spinnaker) to introduce custom stages into orca that support deployment of workloads to Nomad clusters
- [Plugin to trigger pipelines on Azure blob storage artifacts](https://github.com/spinnaker/spinnaker/issues/3776)
- Plugin to automate extraction of key [DORA metrics](https://stelligent.com/2018/12/21/measuring-devops-success-with-four-key-metrics/) from Spinnaker pipelines
- [Plugin to add support for Microsoft Teams notifications to Echo](https://github.com/spinnaker/spinnaker/issues/5826)
- Stage plugin for enabling manual judgements that require data entry 
  - Sometimes approvers for production changes need to manually input information as part of a manual judgement, such as documentation links or further explanation. This plugin could replace or augment the standard manual judgment approval dropdown with a text field in Deck.

## Other Integrations
These may or may not be implementable as plugins
- [Integrate Kafka as a Pub/Sub system in Echo](https://github.com/spinnaker/spinnaker/issues/2117)
- [Add support for AWS CloudWatch metrics in Kayenta](https://github.com/spinnaker/spinnaker/issues/5888)

## Bugfixes & Service Improvements
- [Fix invalid YAML deletion from Manifest Source field upon save](https://github.com/spinnaker/spinnaker/issues/5357)
- Add ingress URLs to the Infrastructure tab
  - Service URLs are shown in the load balancers area, but not ingress URLs. It would be really useful for end users to have the ingress right there to access the deployed app if needed, since many web apps don't use the load balancer URL, but the ingress instead.



