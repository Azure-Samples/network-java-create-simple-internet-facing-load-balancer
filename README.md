---
page_type: sample
languages:
- java
products:
- azure
extensions:
  services: Network
  platforms: java
---

# Getting Started with Network - Create Simple Internet Facing Load Balancer - in Java #


  Azure Network sample for creating a simple Internet facing load balancer -
  <p>
  Summary ...
  <p>
  - This sample creates a simple Internet facing load balancer that receives network traffic on
  port 80 and sends load-balanced traffic to two virtual machines
  <p>
  Details ...
  <p>
  1. Create two virtual machines for the backend...
  - in the same availability set
  - in the same virtual network
  <p>
  Create an Internet facing load balancer with ...
  - A public IP address assigned to an implicitly created frontend
  - One backend address pool with the two virtual machines to receive HTTP network traffic from the load balancer
  - One load balancing rule for HTTP to map public ports on the load
  balancer to ports in the backend address pool
  <p>
  Delete the load balancer
 

## Running this Sample ##

To run this sample:

See [DefaultAzureCredential](https://github.com/Azure/azure-sdk-for-java/tree/main/sdk/identity/azure-identity#defaultazurecredential) and prepare the authentication works best for you. For more details on authentication, please refer to [AUTH.md](https://github.com/Azure/azure-sdk-for-java/blob/main/sdk/resourcemanager/docs/AUTH.md).

    git clone https://github.com/Azure-Samples/network-java-create-simple-internet-facing-load-balancer.git

    cd network-java-create-simple-internet-facing-load-balancer

    mvn clean compile exec:java

## More information ##

For general documentation as well as quickstarts on how to use Azure Management Libraries for Java, please see [here](https://aka.ms/azsdk/java/mgmt).

If you find bug in the sample, please create an issue [here](https://github.com/Azure/azure-sdk-for-java/issues).

Start to develop applications with Java on Azure [here](http://azure.com/java).

If you don't have a Microsoft Azure subscription you can get a FREE trial account [here](http://go.microsoft.com/fwlink/?LinkId=330212).

---

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
