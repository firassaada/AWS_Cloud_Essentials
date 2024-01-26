IAM (Identity and Access Management):
AWS Identity and Access Management (IAM) is a web service that helps you securely control access to AWS resources.
IAM is a GLOBAL service ,not a regional one !!!
It allows you to manage users, groups, roles, and their corresponding permissions within your AWS account.

IAM Users:
IAM users represent individual entities that interact with AWS services. Each IAM user has a unique name and credentials 
(such as a password or access keys) associated with it. 
Users can be assigned specific permissions to access AWS resources. 
IAM users are often used to represent individuals or entities within your organization, and you can manage their access independently.
Users can belong to multiple groups
IAM Groups:
IAM groups are collections of IAM users. Instead of attaching policies directly to individual users,
you can organize users into groups and then attach policies to those groups. 
This makes it easier to manage permissions for multiple users with similar access needs.
When you add a user to a group, they inherit the permissions assigned to that group.
Groups provide a way to apply common policies and permissions to a set of users.
Groups can only contain users , not other groups
IAM Roles:
IAM roles are similar to users, but they are meant to be assumed by other AWS entities or services.
Roles are not associated with a specific identity or credentials; instead, they define a set of permissions that
can be assumed by entities such as AWS services, applications, or other AWS accounts. 
IAM roles are often used to grant temporary permissions to applications or services running on EC2 instances, Lambda functions, or other AWS resources.

IAM policies :
Users or groups can be assigned JSON documents called policies .
![image](https://github.com/firassaada/AWS_Cloud_Essentials/assets/94303698/430cc836-d9ec-4bbb-953f-b76fbf396a5a)





