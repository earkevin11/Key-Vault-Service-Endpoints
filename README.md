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

# Encryption at rest and transit
- Encryption at-rest are encrypted with an encryption key
- 1. Example data stored in a physical server in a data center 
- Encryption in transit means data flowing/moving, it is encrypted so there are no man in the middle attacks.
- 2. User requesting data from an Azure SQL database


# Server-side encryption of Azure Disk Storage
- This is disk encryption for Azure Virtual Machines
- Ensures that data on disks are encrypted at rest
- This also ensures that if the disk got stolen, they would need an encryption key to access the data.
- SSE PMK - means Server Side Encryption Platform Managed Keys where Azure managed the keys


# Encryption with customer managed keys #235
- You can also have customer keys and they can be stored on a Azure Key Vault
- Encryption and decryption is done in the background.

# Azure Disk Encryption
- ADE helps protect and safegaurd your data to meet your organizational security and compliance commitments
- ADE provides VOLUME ENCRYPTION for the OS and data disks of Azure VMs.

# Server Side Encryption
- Aka encryption at-rest or Azure Storage encryption automatically encrypted data stored on Azure managed disks (OS and data disks) when persisting it to the cloud
- This happens in the DATA CENTERS.
