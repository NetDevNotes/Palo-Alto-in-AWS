# Palo-Alto-lab-in-AWS
Tips on spinning up a PA in AWS

1. Create an AWS account [HERE](https://portal.aws.amazon.com/gp/aws/developer/registration/index.html?refid=em_127222)
> Amazon offer a Free Tier which for a period offers access to certain resources at no cost.  Unfortunately the Palo Alto VM is not within the Free Tier.  So you will be charged the hourly cost after the trial period.

>AWS has a [marketplace](https://aws.amazon.com/marketplace) where you can purchase various AMI's (Amazon Machine Images) to launch within your AWS infrastructure. The AWS Marketplace enables qualified partners to market and sell their software to AWS Customers. AWS Marketplace is an online software store that helps customers find, buy, and immediately start using the software and services that run on AWS.

> An AMI is a template that contains the software configuration (operating system, application server, and applications) required to launch an AWS instance. 
2. Log in to AWS and navigate to the [AWS Marketplace](https://aws.amazon.com/marketplace)
3. [Search](https://aws.amazon.com/marketplace/search/results?x=0&y=0&searchTerms=palo+alto) for `palo alto`
4. From the results, click on `VM-Series Next-Generation Firewall Bundle 1` then click on `Continue to Subscribe`
5. Follow the prompts and note the costs.
> To save cost power down your instance when not in use.  
6. At this stage you might get a warning stating your account needs to be verified, if so follow the process.
7. Depending on where you are in the process you might see a button to launch your new Palo Alto instance, you can use this to launch the firewall, or continue below.
8. From the AWS Marketplace, select your name (top right) then `Your Marketplace Account` then `Manage your software subscriptions` 
9. From here you can view and cancel what you are subscribed to:
![Your Software Subscriptions](https://github.com/NetDevNotes/Palo-Alto-lab-in-AWS/blob/master/your_software_subscriptions.png)
10. Navigate to [AWS Console](https://aws.amazon.com/console/)
11. Click on `Services` then `EC2`
12. Click on `Launch Instance`
13. From `Choose an Amazon Machine Image (AMI)`, click on `AWS Marketplace` and search for `palo alto`
14. Find the result `VM-Series Next-Generation Firewall Bundle 1` and click on `Select`
15. Note the pricing and click `Continue`
![Pricing](https://github.com/NetDevNotes/Palo-Alto-lab-in-AWS/blob/master/ami_pricing.png)
16. Fromm `Choose an Instance Type`, scroll down passed the greyed out hardware options to select your hardware platform, the recommended has been selected and is `mx.xlarge`
![Choose an Instance Type](https://github.com/NetDevNotes/Palo-Alto-lab-in-AWS/blob/master/choose_an_instance_type.png)
17. Click `Review and Launch`
18. Note the costs and AMI details.
19. Click `Launch'
20. Create a Key Pair, select the key, acknowledge the agreeement and click `Launch Instances`
> A key pair consists of a public key that AWS stores, and a private key file that you store. Together, they allow you to connect to your instance securely. For Windows AMIs, the private key file is required to obtain the password used to log into your instance. For Linux AMIs, the private key file allows you to securely SSH into your instance. The selected key pair will be added to the set of keys authorized for this instance. 
21. The `Lunch Status` page provides more details while your instance is powering up.
22. Click `View Instances` where you will be taken to the EC2 Instances page, you can see the IP, DNS name and other details here.
![]()

