# AWS.ConnectCampaigns @ default

## Resource AWS.ConnectCampaigns/Campaign@default
* **Valid Scope(s)**: Unknown
### Properties
* **alias**: string (Required): the resource alias
* **name**: string: the resource name
* **properties**: [AWS.ConnectCampaigns/CampaignProperties](#awsconnectcampaignscampaignproperties) (Required): properties of the resource

## AWS.ConnectCampaigns/CampaignProperties
### Properties
* **Arn**: string (ReadOnly, Identifier): Amazon Connect Campaign Arn
* **ConnectInstanceArn**: string (Required): Amazon Connect Instance Arn
* **DialerConfig**: [DialerConfig](#dialerconfig) (Required)
* **Name**: string (Required): Amazon Connect Campaign Name
* **OutboundCallConfig**: [OutboundCallConfig](#outboundcallconfig) (Required)
* **Tags**: [Tag](#tag)[]: One or more tags.

## DialerConfig
### Properties
* **PredictiveDialerConfig**: [PredictiveDialerConfig](#predictivedialerconfig)
* **ProgressiveDialerConfig**: [ProgressiveDialerConfig](#progressivedialerconfig)

## PredictiveDialerConfig
### Properties
* **BandwidthAllocation**: int (Required): The bandwidth allocation of a queue resource.

## ProgressiveDialerConfig
### Properties
* **BandwidthAllocation**: int (Required): The bandwidth allocation of a queue resource.

## OutboundCallConfig
### Properties
* **AnswerMachineDetectionConfig**: [AnswerMachineDetectionConfig](#answermachinedetectionconfig)
* **ConnectContactFlowArn**: string (Required): The identifier of the contact flow for the outbound call.
* **ConnectQueueArn**: string (Required): The queue for the call. If you specify a queue, the phone displayed for caller ID is the phone number specified in the queue. If you do not specify a queue, the queue defined in the contact flow is used. If you do not specify a queue, you must specify a source phone number.
* **ConnectSourcePhoneNumber**: string: The phone number associated with the Amazon Connect instance, in E.164 format. If you do not specify a source phone number, you must specify a queue.

## AnswerMachineDetectionConfig
### Properties
* **EnableAnswerMachineDetection**: bool (Required): Flag to decided whether outbound calls should have answering machine detection enabled or not

## Tag
### Properties
* **Key**: string (Required): The key name of the tag. You can specify a value that is 1 to 128 Unicode characters in length and cannot be prefixed with aws:. You can use any of the following characters: the set of Unicode letters, digits, whitespace, _, ., /, =, +, and -. 
* **Value**: string (Required): The value for the tag. You can specify a value that's 1 to 256 characters in length.

