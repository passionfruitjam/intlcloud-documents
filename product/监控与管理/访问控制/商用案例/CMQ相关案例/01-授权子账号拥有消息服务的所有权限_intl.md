### Grant a sub-account full permissions to use messaging services

For example, we have a sub-account of the enterprise account CompanyExample called Developer, and it requires full permissions to read and write the message queue in CompanyExample. The message queue can be either topic model or queue model based.

Solution A:

The enterprise account CompanyExample directly authorizes the preset policies QCloudCmqQueueFullAccess and QCloudCmqTopicFullAccess to the sub-account Developer. For more information on authorization, see [Authorization Management](https://cloud.tencent.com/document/product/378/8961).

Solution B:

Step 1: Create the following policy using policy syntax
```
 {
    "version": "2.0",
    "statement":
     {
         "effect": "allow",
         "action": ["cmqtopic:*","camqueue:*"]
         "resource": "*"
     }
}
```
Step 2: Authorize the policy to the sub-account. For more information on authorization, see [Authorization Management](https://cloud.tencent.com/document/product/378/8961).


