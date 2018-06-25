---
services: virtual-network,load-balancer
platforms: java
author: martinsawicki
---

## Getting Started with Network - Create Simple Internet Facing Load Balancer - in Java ##


  Azure Network sample for creating a simple Internet facing load balancer -
 
  Summary ...
 
  - This sample creates a simple Internet facing load balancer that receives network traffic on
    port 80 and sends load-balanced traffic to two virtual machines
 
  Details ...
 
  1. Create two virtual machines for the backend...
  - in the same availability set
  - in the same virtual network
 
  Create an Internet facing load balancer with ...
  - A public IP address assigned to an implicitly created frontend
  - One backend address pool with the two virtual machines to receive HTTP network traffic from the load balancer
  - One load balancing rule for HTTP to map public ports on the load
    balancer to ports in the backend address pool

  Delete the load balancer
 

## Running this Sample ##

To run this sample:

Set the environment variable `AZURE_AUTH_LOCATION` with the full path for an auth file. See [how to create an auth file](https://github.com/Azure/azure-libraries-for-java/blob/master/AUTH.md).

    git clone https://github.com/Azure-Samples/network-java-create-simple-internet-facing-load-balancer.git

    cd network-java-create-simple-internet-facing-load-balancer

    mvn clean compile exec:java

## More information ##

[http://azure.com/java](http://azure.com/java)

If you don't have a Microsoft Azure subscription you can get a FREE trial account [here](http://go.microsoft.com/fwlink/?LinkId=330212)

---

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.