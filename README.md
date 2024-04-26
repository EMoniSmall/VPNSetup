# Virtual Private Networks: Setting Up and Using VPNs

> [!Note]
> What is a VPN?
> A VPN or virtual private network is a secure connection that encrypts internet traffic and routes it through a remote server. This masks IP addresses and enhances privacy by making it appear that you're physically in a different location. VPNs are used to protect sensitive data, bypass geographical restrictions and enhance online security and anonymity. Think of VPNs as a safe and secure tunnel you can send data through.

> [!Important]
> You'll need to download a free version of [Proton VPN](https://protonvpn.com/). You'll also be creating an Azure VM to also practice with. For assistance creating an Azure VM, refer to the [Azure Crash Course: VM Section](https://github.com/EMoniSmall/azurecrashcourse?tab=readme-ov-file#virtual-machines--).

<b>Common Uses for VPNs</b>

- Can be used in public such as cafes, airports or hotels where there are public Wi-Fi networks.

- Reduces latency and DDoS attacks while gaming online.

- Can prevent bandwidth throttling when streaming or downloading.

- Can conceal IP address to prevent websites and advertisers from tracking your activities.

<h2>Building an Intuition for VPNs</h2>

 Step 1: First visit [WhatIsMyIPAddress.com](WhatIsMyIPAddress.com) and take note of your IP Address. 

 Step 2: Visit [Portal.Azure.com](Portal.Azure.com) and create a VM using Windows 10. 

 > [!Important]
> When selecting the Region for your VM, select a region other than where you live.

Step 3: Retrieve the Public IP for your new VM and Connect to it via Remote Desktop Connection.

Step 4: Within your VM, visit [WhatIsMyIPAddress.com](WhatIsMyIPAddress.com) and take note of the VM's IP Address.

> [!Note]
> If your VM region was set in another country, such as Japan, you'll see that any google searches you make may come up in Japanese since the server believes the VM is physically there.

<h3>VPN Setup</h3>

> [!Important]
> If you haven't already, set-up your free [Proton VPN account](protonvpn.com).

 Step 1: Inside your VM, log into Proton VPN and download the free version. (Default installation is fine.)

> [!Note]
> Installing and using the VPN may interupt the connection to the VM. 

Step 2: Once download, open the application and attempt to connect to a server. 

![image](https://github.com/EMoniSmall/VPNSetup/assets/166156618/07cf4e65-9efc-42d9-aa2c-7749d7576f50)

> [!Note] At the time of making this guide, ProtonVPN no longer allows you to pick and choose which free VPN server you can use. Ideally, attempt to get connected to a VPN server in a different country. You can do this by hitting the "Change Server" option.
>
> ![image](https://github.com/EMoniSmall/VPNSetup/assets/166156618/f04cc7e5-a755-40b9-bdb6-e54d54fbc506)

Step 3: Once you have connected to a VPN server inside your VM, return to WhatIsMyIPAddress.com and refresh. Compare it to the VPN you noted down for your VM and see how your VM's "location" has changed. 

> [!Note]
> When using a Remote Desktop Connection, using a VM is almost similar to using a VPN as you're connected to the VM from a different location. 
