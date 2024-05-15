<h1>Creating an Active Directory Domain Server</h1>

<h2>Overview</h2>
This project aims to provide a comprehensive guide and resources for setting up an Active Directory Domain Server (AD DS) environment within Oracle VM VirtualBox. Active Directory is a crucial component in many enterprise networks, facilitating centralized management of users, groups, and resources. By utilizing virtualization technology, users can easily create and manage test environments for learning, development, or testing purposes.

<h2>Environments and Tools</h2>

- Windows Server 2019

- Windows 10 Pro (2H22)
  
- Configuration of Essential Services: DHCP (Dynamic Host Configuration Protocol), DNS (Domain Name System), RAS (Routing and Remote Access), and NAT (Network Address Translation) to support AD DS functionality.

Let's get started!
  
<h2>Network Diagram</h2>

Below I have created a basic network diagram to show how the system will connect. It is useful to create a template like this before starting a large project because it can be referenced when setting up our key network protocols. While this netork lacks key detection and prevention security controls, I will show you how to implement these in a later tutorial. For now lets stick to the already complex task of setting up an active directory domain server.

![Diagram](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/Network%20Diagram.png)

I included information such as a rough scope for our DHCP. We will be using two NIC's to create a private network for our domain. The internal NIC allows communication between devices in our virtual subnet. The external NIC will provide internet access for the private network. Our AD DS server will use DHCP to automatically assign private IP addresses to devices on our internal network. The domain controller will have its ip address assigned to it by the home router.

<h2>Setting up Windows Server 2019</h2>

![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/0.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/1.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/2.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/3.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/4.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/5.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/6.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/7.png)

<h2>Configuring TCP/IPv4</h2>

![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/8.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/10.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/11.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/12.png)

<h2>Installing Active Directory Domain Services</h2>

![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/13.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/14.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/15.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/16.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/17.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/18.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/19.png)

<h2>Creating Active Directory Objects</h2>

![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/20.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/21.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/22.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/23.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/24.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/25.png)

<h2>Setting up RAS and NAT</h2>

![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/26.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/27.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/28.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/29.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/30.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/31.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/32.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/33.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/34.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/35.png)


<h2>Setting up DHCP</h2>

![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/26.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/36.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/37.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/38.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/39.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/40.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/41.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/42.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/43.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/44.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/45.png)

<h2>Creating our first Client</h2>

![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/46.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/47.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/48.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/49.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/50.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/51.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/52.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/53.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/54.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/55.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/56.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/57.png)

<h2>Connecting our new Client to our Domain</h2>

![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/58.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/59.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/60.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/61.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/62.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/63.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/64.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/65.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/66.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/67.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/69.png)
![step](https://github.com/nicknava1/AD-DS/blob/main/Active%20Directory/70.png)
