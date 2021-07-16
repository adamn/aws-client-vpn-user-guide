# Getting started with Client VPN<a name="user-getting-started"></a>

Before you can establish a VPN session, your Client VPN administrator must create and configure a Client VPN endpoint\. Your administrator controls which networks and resources you can access when you establish a VPN session\. You then use a VPN client application to connect to a Client VPN endpoint and establish a secure VPN connection\.

If you're an administrator who needs to create a Client VPN endpoint, see the [AWS Client VPN Administrator Guide](https://docs.aws.amazon.com/vpn/latest/clientvpn-admin/)\.

**Topics**
+ [Prerequisites](#install-prereq)
+ [Step 1: Get a VPN client application](#install-client)
+ [Step 2: Get the Client VPN endpoint configuration file](#get-config-file)
+ [Step 3: Connect to the VPN](#import-connect)
+ [Use the self\-service portal](self-service-portal.md)

## Prerequisites<a name="install-prereq"></a>

To establish a VPN connection, you must have the following:
+ Access to the internet
+ A supported device
+ For Client VPN endpoints that use SAML\-based federated authentication \(single sign\-on\), one of the following browsers:
  + Apple Safari
  + Google Chrome
  + Microsoft Edge
  + Mozilla Firefox

## Step 1: Get a VPN client application<a name="install-client"></a>

You can connect to a Client VPN endpoint and establish a VPN connection using the AWS provided client or another OpenVPN\-based client application\. 

The AWS provided client is a supported on Windows, macOS, Ubuntu 18\.04 LTS, and Ubuntu 20\.04 LTS\. You can download the client at [AWS Client VPN download](https://aws.amazon.com/vpn/client-vpn-download/)\.

Alternatively, download and install an OpenVPN client application on the device from which you intend to establish the VPN connection\.

## Step 2: Get the Client VPN endpoint configuration file<a name="get-config-file"></a>

You must get the Client VPN endpoint configuration file from your administrator\. The configuration file includes the information about the Client VPN endpoint and the certificates that are required to establish a VPN connection\.

Alternatively, if your Client VPN administrator has configured a self\-service portal for the Client VPN endpoint, you can download the latest version of the AWS provided client and the latest version of the Client VPN endpoint configuration file yourself\. For more information, see [Use the self\-service portal](self-service-portal.md)\.

## Step 3: Connect to the VPN<a name="import-connect"></a>

Import the Client VPN endpoint configuration file to the AWS provided client or to your OpenVPN client application and connect to the VPN\. For steps to connect to a VPN, see the following topics:
+ [Connect using an AWS provided client](connect-aws-client-vpn-connect.md)
+ [Connect using an OpenVPN client](connect.md)

For Client VPN endpoints that use Active Directory authentication, you will be prompted to enter your user name and password\. If multi\-factor authentication \(MFA\) has been enabled for the directory, you will also be prompted to enter your MFA code\.

For Client VPN endpoints that use SAML\-based federated authentication \(single sign\-on\), the AWS provided client opens a browser window on your computer\. You'll be prompted to enter your corporate credentials before you can connect to the Client VPN endpoint\.