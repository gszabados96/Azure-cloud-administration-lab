# Azure-cloud-administration-lab
This lab is for creating and maintaining a Cloud Infrastructure.

# Key objectives:
    1, Deploy and maintain an Azure VM within a controlled environment.
    2, Creating NSG rules to restrict accesses.
    3, Enabling monitoring for check how visible are the operations.

# Focus:
    1, Resource organization.
    2, Network security.
    3, Monitoring and alerting.

# Deployed resources:
    1, Azure Resource Group
    2, Virtual Network and Subnet(s)
    3, Windows Server VM
    4, Network Security Group
    5, Azure Monitor Alert rule

# Actions taken:
    03/02/2026:
       1, I've investigated and found that I had 3 active resource groups (HoneyPot_Lab, NetworkWatcherRG and
            RG_Web_Server) -> I've deleted the groups to save costs are resources.
       2, Created a Virtual Machine in Azure named gszabadosTesting, and also configured it to be in a nearly
            region with good availability. 
            2/a Username and pw has been added with inbound ports 22
            2/b Default image has been chosen for the disk
            2/c An already existing vnet has been added.
            2/d Custom rules have been enabled.
       3, Created a Virtual Network named gszabadosVnet
            3/a Allowed Virtual Network Encryption and Azure Firewall (gszabadosVnet-Firewall)
            3/b When setting up the IP addresses, modified the default from 0.0.0.0 to 123.235.0.0

# Lessons learned:
    1, When trying to delete a resource group, I've encountered this EM: "The resource group HoneyPot_Lab is
        locked and can't be deleted." -> Manually unlocked and deleted the resource.


# Author
    Gyula Szabados
    LinkedIn Profile: www.linkedin.com/in/gyula-szabados-83b889277