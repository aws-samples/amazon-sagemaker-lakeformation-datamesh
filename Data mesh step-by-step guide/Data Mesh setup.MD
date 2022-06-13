#  Set up resources with AWS CloudFormation

This repository accompanies the [Build and train ML models with a data mesh design pattern on AWS]() blog post. we provide **Three** [AWS Cloudformation](https://aws.amazon.com/cloudformation/) templates in this post: for the producer account, central account, and consumer account. Deploy the CloudFormation templates in the order of producer, central, and consumer, because there are dependencies between the templates.

### The CloudFormation template for the central account generates the following resources:
* Two IAM users: 
  * `DataMeshOwner`
  * `ProducerSteward`
* Grant `DataMeshOwner` as the LakeFormation Admin.
* One IAM role: 
  * `LFRegisterLocationServiceRole`
* Two IAM policies: 
  * `ProducerStewardPolicy`
  * `S3DataLakePolicy`
* Create databases `credit-card` for `ProducerSteward` to manage Data Catalog
* Share the data location permission for producer account to manage Data Catalog
