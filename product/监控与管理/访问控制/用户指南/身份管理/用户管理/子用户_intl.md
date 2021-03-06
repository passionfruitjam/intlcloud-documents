## Overview
Sub-users are entities created by the root account. A sub-user is assigned an ID and credentials, and is able to log in to and configure console independently and has the access to APIs.

## Operation Guide

### Create a sub-user
1. Log in to the Tencent Cloud console, go to [User](https://console.cloud.tencent.com/cam), click **New User** -> **Sub-User**, as shown below:
![](https://main.qcloudimg.com/raw/ea2c83f453f040868d74cebde326ece2.png)

2. Enter the user information. During this process, you can create sub-users in batches, set access type and console password or perform other operations, as shown below:
![](https://main.qcloudimg.com/raw/4af2c64e456a66c71aeba544237c5aaa.png)

3. Set permission.  After associated with a policy, the sub-user will be automatically granted the permissions described in that policy. You can give sub-user permission in 3 different ways:
 - Add sub-user to a user group: This is the best way to manage permissions for users with different roles and functions. You can grant permissions to a sub-user by adding the sub-user to an existing user group or creating a new user group. After that, the sub-user will be associated with the policies of the user group.
![](https://main.qcloudimg.com/raw/42203e02f8db3e3f380d7b41b133885b.png)
 - Copy the permissions of an existing user: click **Copy Existing User's Permissions** and select the user whose permissions you want to copy, then you can associate the sub-user with the policies of that user.
![](https://main.qcloudimg.com/raw/e144d026b601ef06f0b678905ec9dbaa.png)
 - Use the policy list: Click **Grant Permissions from Policy List**, and then select the policies you want to associate with the sub-user.
 ![](https://main.qcloudimg.com/raw/ec45ef82b8f31d6707d8873cc5485155.png)
4. You can email the complete information to the mailbox, or save some of the information to a local Excel file, as shown below:
![](https://main.qcloudimg.com/raw/5538d2b037b8d0299c6f96185e85f828.png)

5. Click **Done**.

### Associate a sub-user with policies

#### Direct association
1. Log in to the Tencent Cloud console, go to [User](https://console.cloud.tencent.com/cam) and select the sub-user you want to associate the polices with, then click **Authorize** in the **Operation** column, as shown below:
![](https://main.qcloudimg.com/raw/def984e04ba312d066f5ced32996cb99.png)
2. Select the policies to be associated, and then click **OK**.
![](https://main.qcloudimg.com/raw/0ed5b135fe498eb017552a9014b29893.png)

#### Association with policies by joining groups
1. Log in to the Tencent Cloud console, go to [User](https://console.cloud.tencent.com/cam), select the sub-user you want to authorize, and then click **More** -> **Add to Group** in the **Operation** column.
![](https://main.qcloudimg.com/raw/ccd8ed71ab1e2414adccc07d699bbe54.png)
2. Select the user group to which you want to add the sub-user, and then click **OK**.


### Disassociate a sub-user from policies

#### Direct disassociation
1. Log in to the Tencent Cloud console, go to [User](https://console.cloud.tencent.com/cam), select the sub-user you want to disassociate from the policies, and then click the sub-user name to enter the details page.
![](https://main.qcloudimg.com/raw/7acf69885801de4d444955f3315fe4cf.png)
2. Click **Associated Policies**, choose the policies to be disassociated in the list, and then click **Disassociate** on the right.
![](https://main.qcloudimg.com/raw/8f39787d4168aca9cb49856f0b2579be.png)
3. Click **Disassociate**.

#### Remove a sub-user from a user group
1. Log in to the Tencent Cloud console, go to [User](https://console.cloud.tencent.com/cam), select the sub-user you want to disassociate from the policies, and then click the sub-user name to enter the detail page.
![](https://main.qcloudimg.com/raw/7acf69885801de4d444955f3315fe4cf.png)
2. Click **Associated Policies**, in the list choose the policies you want to disassociate, and then click **Disassociate** on the right.
![](https://main.qcloudimg.com/raw/bf4de0304257aab985745b7e456c40c7.png)
3. Click **Disassociate** to remove the sub-user from the user group. The sub-user is now disassociated from the policies of that user group.

### Subscribe a sub-user to messages
1. Log in to the Tencent Cloud console, go to [User](https://console.cloud.tencent.com/cam), select the sub-user for whom you want to subscribe to messages service, and then click **More** -> **Subscribe to Messages** in the **Operation** column, as shown below:
![](https://main.qcloudimg.com/raw/110fe3ebd376969a1b18f81f287ee88b.png)
2. Select the desired message type and click **OK**.
![](https://main.qcloudimg.com/raw/1eac93c0efd19c26e0ca1e3a1e637b75.png)

### View sub-user information in **User List** -> **Details**

1. Log in to the Tencent Cloud console, go to [User](https://console.cloud.tencent.com/cam), select the sub-user you want to view, and then click **details** on the left, as shown below: ![](https://main.qcloudimg.com/raw/4413929aa2d843861a5512da4a27d437.png)


### Search for sub-users using search box
1. Log in to the Tencent Cloud console, go to [User](https://console.cloud.tencent.com/cam), enter the keyword in the search box at the upper right corner, and then click **search**. 
![](https://main.qcloudimg.com/raw/21545d7d3da888f878dda5d82c75a8e9.png)
>The search box supports multi-keyword search (separated by a space). You can search for sub-users by using keywords such as username, ID, mobile number, email and remarks.



### Delete a sub-user

#### Delete a single sub-user
1. Log in to the Tencent Cloud console, go to [User](https://console.cloud.tencent.com/cam), select the sub-user you want to delete, and then click **More** -> **Delete** in the **Operation** column, as shown below:
![](https://main.qcloudimg.com/raw/fc3a8a73f4ef0f53f8ad3a2a7b8d4cd2.png)

2. Click **Delete**.


#### Delete multiple sub-users
1. Log in to the Tencent Cloud console, go to [User](https://console.cloud.tencent.com/cam), in the user list select multiple sub-users you want to delete, and then click **Delete** at the upper left corner, as shown below:
![](https://main.qcloudimg.com/raw/983a54ffdf83dcd0d4b9da6a7f746f27.png)

2. Click **Delete**.

