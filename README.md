# introduction_to_cloud_computing_and_aws
Udacity instructions for aws redshif


## Steps to delete a cluster are:

1. On the Clusters page of your Amazon Redshift console, click on the check-box next to your cluster name. Then click on the Actions drop-down button on top → select Delete.

<img width="1059" alt="aaaaaaaaaaa" src="https://user-images.githubusercontent.com/1679821/149808240-18471d9a-d3e3-4bdb-a071-7df95483749f.png">


Delete a cluster

2. You can choose to not Create final snapshot, and click on the Delete cluster button.

<img width="608" alt="screenshot-2021-03-26-at-4 10 50-pm" src="https://user-images.githubusercontent.com/1679821/149808555-203a69a0-0778-42b1-a41e-9e93738531d8.png">

Prompt before deleting the cluster

3. Your cluster will change it's status to deleting, and then disappear from your Cluster list once it's finished deleting. You'll no longer be charged for this cluster.



## S3 - Create a Bucket


### Create a Bucket
1 . Navigate to the S3 dashboard, and click on the Create bucket button. It will launch a new wizard.

S3 service → Buckets dashboard.
View all of the S3 buckets in your account
(S3 is a global service, not a region-specific).

We create a bucket first, and later we upload files and folders to it.

2. General configuration
Provide the bucket-name and the region where you want to locate the bucket. The bucket name must be unique worldwide, and must not contain spaces or uppercase letters.

Create a bucket - Provide general details

3. Public Access settings
You can choose public visibility. Let's uncheck the Block all public access option.

Create a bucket - Make it public

4. Bucket Versioning and Encryption
Bucket Versioning - Keep it disabled.
Encryption - If enabled, it will encrypt the files being stored in the bucket.
Object Lock - If enables, it will prevent the files in the bucket from being deleted or modified.

Create a bucket - Provide additional details

In the snapshots above, we have created a public bucket. Let's see how to upload files and folders to the bucket, and configure additional settings.

Upload File/Folders to the Bucket
From the S3 dashboard, click on the name of the bucket you have created in the step above.


Details of an existing bucket. Upload files/folders to this bucket.

In the snapshot above, it shows that the bucket is in the Region: US East (Ohio) us-east-2, and it has a unique Amazon resource name (ARN): arn:aws:s3:::mtvbucket. You can view more details of the bucket, in the tabs next to the bucket overview: Objects, Properties, Permissions, Metrics, Management, and Access points. Leet's upload a sample file to the bucket:

Click on the Upload button to upload files and folders into the current bucket. In the snapshot below, we have uploaded a Sample.txt file.

A sample file in the bucket

Click on the file name to view the file-specific details, as shown below.

Details of an individual file (object)

Details of an Existing Bucket
1. Properties
There are several properties that you can set for S3 buckets, such as:

Bucket Versioning - Allows you to keep multiple versions of an object in the same bucket.
Static website hosting - Mark if the bucket is used to host a website. S3 is a very cost-effective and cheap solution for serving up static web content.
Requester pays - Make the requester pays for requests and data transfer costs.
Server access logging - Log requests for access to your bucket.
Permissions
It shows who has access to the S3 bucket, and who has access to the data within the bucket. In the example snapshots above, the bucket is public, meaning anyone can access it. Here, we can write an access policy (in JSON format) to provides access to the objects stored in the bucket.

2. Metrics
View the metrics for usage, request, and data transfer activity within your bucket, such as, total bucket size, total number of objects, and storage class analysis.

3. Management
It allows you to create life cycle rules to help manage your objects. It includes rules such as transitioning objects to another storage class, archiving them, or deleting them after a specified period of time.

4. Access points
Here, you can create access endpoints for sharing the bucket at scale. Using an endpoint, you can perform all regular operations on the bucket.

;
