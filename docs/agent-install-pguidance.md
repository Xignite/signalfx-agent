# Install and Configure the Smart Agent

SignalFx Smart Agent collects infrastructure metrics, Kubernetes cluster
data, and Microservice APM data from you systems and sends it to
SignalFx for analysis.

## Choose an install type that meets your needs

SignalFx offers several different installation mechanisms to match
your needs. The following list organizes the mechanisms by use case:

**Testing Splunk Observability Suite:**

* **Testing infrastructure metrics:** I want to install and configure Smart Agent on a few test hosts, so I can
  send monitoring data such as cpu metrics to Splunk and look at it
  using observability tools such as charts.

  For Linux hosts that have Internet access, follow the instructions in the topic [Install Using Linux Packages](pguidance/agent-install-packages.md)

  For Linux hosts that don't have Internet access, follow the instructions in the topic [Install to Linux Using gzip File](pguidance/agent-install-standalone-linux.md)

  For Windows hosts, use [Install to Windows Using zip File](pguidance/agent-install-standalone-windows.md)

  For a single host, follow the instructions in the Setup section of the topic [Quick Install](./quick-install.md).

* **Testing Kubernetes observability:** I want to install and configure Smart Agent in a test Kubernetes system,
  so I can send Kubernetes monitoring data to Splunk and navigate through it using Kubernetes Navigator.

  If you have `helm` installed, follow the instructions in the topic [Install Using helm](pguidance/agent-k8s-install-helm.md).

  If you don't have `helm`, you can install Smart Agent with `kubectl`. Follow the  
  instructions in the topic [Install Using kubectl](pguidance/agent-k8s-install-kubectl.md).

* Testing Microservices APM (**µAPM**) observability:  I want to install and configure Smart Agent in a test µAPM system,
  so I can send monitoring data to Splunk and navigate through it using µAPM tools.

  If you're running your microservices in Docker outside of Kubernetes, follow the instructions in the topic
  [SignalFx Agent Docker Image](https://github.com/signalfx/signalfx-agent/tree/master/deployments/docker).

  If you're running your microservices in Kubernetes, install and configure Smart Agent according to the instructions
  in the previous point, **Testing Kubernetes observability**.

**Beta test and production installations:**


* **Infrastructure monitoring:** I want to install and configure Smart Agent in a beta or production system, so I can
  send monitoring data such as cpu metrics to Splunk and look at it using observability tools such as charts.
  If you're installing to Amazon Web Services (**AWS**) Elastic Container Service (**ECS**), follow the instructions
  in the topic [Install to AWS ECS](pguidance/agent-install-awsecs.md).

  If you have a configuration management tool such as `puppet`, refer to the topic [Install Smart Agent using Configuration Management](pguidance/agent-install-config-mgmt.md) to see
  if Splunk provides a compatible Smart Agent installation package.

  **For Linux:**

  If you don't have a configuration management tool, follow the instructions in the topic [Install Using Linux Packages](pguidance/agent-install-packages.md) for each host machine in your system.

  For Linux hosts that don't have Internet access, follow the instructions in the topic [Install to Linux Using gzip File](pguidance/agent-install-standalone-linux.md)


  **For Windows:**

  If you don't have a configuration management tool, follow the instructions in the topic [Install to Windows Using zip File](pguidance/agent-install-standalone-windows.md) for each host machine in your system.

* **Kubernetes monitoring:** I want to install and configure Smart Agent in a beta or production Kubernetes system,
  so I can send Kubernetes monitoring data to Splunk and navigate through it using Kubernetes Navigator.

* **µAPM monitoring:** I want to install and configure Smart Agent in a beta or production µAPM system, so I can
  send µAPM monitoring data to Splunk and navigate through it using µAPM tools.