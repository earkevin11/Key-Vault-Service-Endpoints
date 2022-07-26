# Key-Vault-Service-Endpoints

# What are service endpoints?
- They help with secure communication between virtual machines located in an Azure virtual network and resources that are deployed apart of the subscription.
- You can use service endpoints and use it as a middle men.
- First step to use service endpoint is to enable the service endpoint from the Azure virtual network AND the Azure resource including the firewall


# Note: Azure Key Vault is a public service so everyone can access it.
- Admins can configure and limit access based on networks/IP

# Add a service endpoint
- This extends the virtual network onto a particular service, in this case, it is the key vault. 
- Navigate to the virtual network > service endpoints > Microsoft.KeyVault > Select the subnet
- This is a more secure communication between the Azure Keyvault and the Azure network.


<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/181098316-54fcefae-769a-41d1-86b3-2562fd2d2a5a.png" height="50%" width="50%" alt="key vault"/>

<p/>
