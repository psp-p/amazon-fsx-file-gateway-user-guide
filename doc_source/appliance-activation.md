--------

Amazon S3 File Gateway documentation has been moved to [What is Amazon S3 File Gateway?](https://docs.aws.amazon.com/filegateway/latest/files3/WhatIsStorageGateway.html)

Volume Gateway documentation has been moved to [What is Volume Gateway?](https://docs.aws.amazon.com/storagegateway/latest/vgw/WhatIsStorageGateway.html)

Tape Gateway documentation has been moved to [What is Tape Gateway?](https://docs.aws.amazon.com/storagegateway/latest/tgw/WhatIsStorageGateway.html)

--------

# Activating your hardware appliance<a name="appliance-activation"></a>

After configuring your IP address, you enter this IP address in the console on the **Hardware** page, as described following\. The activation process validates that your hardware appliance has the appropriate security credentials and registers the appliance to your AWS account\.

You can choose to activate your hardware appliance in any of the supported AWS Regions\. For a list of supported AWS Regions, see [Storage Gateway Hardware Appliance Regions](https://docs.aws.amazon.com/general/latest/gr/sg.html#sg-hardware-appliance) in the *AWS General Reference*\.

**To activate your appliance for the first time or in an AWS Region where you have no gateways deployed**

1. Sign in to the AWS Management Console and open the Storage Gateway console at [AWS Storage Gateway Management Console](https://console.aws.amazon.com/storagegateway/home) with the account credentials to use to activate your hardware\.

   If this is your first gateway in an AWS Region, you see a splash screen\. After you create a gateway in this AWS Region, the screen no longer displays\.
**Note**  
For activation only, the following must be true:  
Your browser must be on the same network as your hardware appliance\.
Your firewall must allow HTTP access on port 8080 to the appliance for inbound traffic\.

1. Choose **Get started** to view the Create gateway wizard, and then choose **Hardware Appliance** on the **Select host platform** page, as shown following\.

1. Choose **Next** to view the **Connect to hardware** screen shown following\.

1. For **IP Address** in the **Connect to hardware appliance** section, enter the IPv4 address of your appliance, and then choose **Connect** to go to the Activate Hardware screen shown following\.

1. For **Hardware name**, enter a name for your appliance\. Names can be up to 255 characters long and can't include a slash character\.

1. For **Hardware time zone**, enter your local settings\.

   The time zone controls when hardware updates take place, with 2 a\.m\. local time used as the time for updates\.
**Note**  
We recommend setting the time zone for your appliance as this determines a standard update time that is out of the usual working day window\.

1. \(Optional\) Keep the **RAID Volume Manager** set to **ZFS**\.

   ZFS is used as the RAID volume manager on the hardware appliance to provide better performance and data protection\. ZFS is a software\-based, open\-source file system and logical volume manager\. The hardware appliance is specifically tuned for ZFS RAID\. For more information on ZFS RAID, see the [ZFS](https://en.wikipedia.org/wiki/ZFS) Wikipedia page\.

1.  Choose **Next** to finish activation\.

A console banner appears on the **Hardware appliance overview** page indicating that the hardware appliance has been successfully activated, as shown following\.

At this point, the appliance is associated with your account\. The next step is to launch a file, tape, or cached Volume Gateway on your appliance\.

![\[Image NOT FOUND\]](http://docs.aws.amazon.com/filegateway/latest/filefsxw/images/appliance-activation-final.png)





**Next step**

[Creating a gateway](appliance-launch-gateway.md)