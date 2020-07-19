# Development Environments for Spinnaker Gardening Days

Gardening participants have options when it comes to development environments, and one goal of the event is to help participants become comfortable setting up a development environment and workflow for Spinnaker. 

### Managed Development Environments & AWS Compute Sponsorship 
For the July Gardening Days, Armory will provide a managed sandbox environment in AWS EKS, thanks to our compute sponsor, Amazon. Each Gardening participant who enrolls in the New Spin Contributor Workshop or requests a sandbox via Slack is assigned their own namespace in the cluster, with access to that namespace only. Participants can follow the workshop [video](https://youtu.be/Sb5CO6RQx_Q) and [guide](https://spinnaker.io/community/gardening/spin-contrib/) to install Spinnaker there, and then use Telepresence to set up a local development environment for Spinnaker services that is connected to the remote K8S cluster. 

To request a sandbox, @ mention @Fernando Freire in [#gardening-training](https://spinnakerteam.slack.com/archives/C011CAW95SP), and we'll create one for you to develop in.

### Alternative Development Environment Creation
There are a number of ways to create a development environment for Spinnaker, including:
- Use [Minnaker](https://github.com/armory/minnaker), an all-in-one quickstart developed at Armory
- Install and configure the Spinnaker services on your local machine
- Install Spinnaker on Kubernetes running in the location of your choice

Read the [documentation for these methods](https://spinnaker.io/community/gardening/dev-environment/) in the Gardening area on the Spinnaker website. 
