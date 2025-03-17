# Azure Infrastructure Deployment

During the infrastructure creation, I worked with various Azure resources to ensure secure deployment. The process involved setting up a virtual machine, configuring networking, and applying security measures to allow controlled access though ssh. Below are the key components used.

## Components

### Resource group
> Logical container for all associated resources.

### Virtual Machine (VM)
> The VM is the core component, deployed with a minimal configuration for cost efficiency and lightweight performance. The chosen OS is Ubuntu 24.04 LTS and size is Standard_B1ls for lowest prize. Authentication method was set to ssh public key to ensure security.

### Virtual Network (VNet)
> The VNet provides a private network environment, isolating resources for better security and internal communication.

### Network Interface (NIC)
> The NIC acts as the bridge between the VM and the network, allowing connectivity while enforcing security policies. It's required for NSG rules to be applied.

### Network Security Group (NSG)
> The NSG acts as a firewall, restricting traffic to only necessary services while keeping other ports closed.

### Public IP
> Public IP is assigned to allow external access to the VM.

### SSH Public Key
> This key ensures passwordless and secure access to the VM, avoiding common security risks from weak credentials.
