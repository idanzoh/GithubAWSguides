# AWS Systems Manager Lab Guide
## Task 1: Generate inventory lists for managed instances
You can use Fleet Manager, a capability of Systems Manager, to collect operating system information, application information, and metadata from EC2 instances, on-premises servers, or virtual machines in a hybrid environment. You can also use Fleet Manager to query metadata to quickly understand which instances are running the software and configurations that your software policy requires and which instances you need update.

In this task, you use Fleet Manager to gather inventory from an EC2 instance.

In the AWS Management Console, in the  search box, enter Systems Manager and press Enter. This option takes you to the Systems Manager console page.

In the left navigation pane, for Node Management, choose Fleet Manager.

Choose the Account management dropdown list, and choose Set up inventory.

To create an association that collects information about software and settings for your managed instance, choose the following options:

In the Provide inventory details section, for Name, enter Inventory-Association

In the Targets section, choose the following options:

For Specify targets by, choose Manually selecting instances.
Select the row for Managed Instance.
Leave the other options as the default settings.

Choose Setup Inventory

A banner with the message "Setup inventory request succeeded" appears on the Fleet Manager page. Inventory, a capability of Systems Manager, now regularly inventories the instance for the selected properties.

Choose the Node ID link, which directs you to the Node overview.

Choose the Inventory tab.

This tab lists all of the applications in the instance. Take a moment to review the installed applications and other options in the Inventory type dropdown list.

You have successfully created a Systems Manager inventory association for your instance. Using Inventory, you can review and validate software configurations on your instances without needing to connect to each instance by using SSH.