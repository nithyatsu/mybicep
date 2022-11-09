# AWS.ApiGatewayV2 @ default

## Resource AWS.ApiGatewayV2/Api@default
* **Valid Scope(s)**: Unknown
### Properties
* **name**: string (Required): the resource name
* **properties**: [AWS.ApiGatewayV2/ApiProperties](#awsapigatewayv2apiproperties): properties of the resource

## Resource AWS.ApiGatewayV2/Model@default
* **Valid Scope(s)**: Unknown
### Properties
* **name**: string (Required): the resource name
* **properties**: [AWS.ApiGatewayV2/ModelProperties](#awsapigatewayv2modelproperties) (Required): properties of the resource

## Resource AWS.ApiGatewayV2/VpcLink@default
* **Valid Scope(s)**: Unknown
### Properties
* **name**: string (Required): the resource name
* **properties**: [AWS.ApiGatewayV2/VpcLinkProperties](#awsapigatewayv2vpclinkproperties) (Required): properties of the resource

## AWS.ApiGatewayV2/ApiProperties
### Properties
* **ApiEndpoint**: string (ReadOnly)
* **ApiId**: string (ReadOnly)
* **ApiKeySelectionExpression**: string
* **BasePath**: string (WriteOnly)
* **Body**: [Api_Body](#apibody) (WriteOnly)
* **BodyS3Location**: [BodyS3Location](#bodys3location) (WriteOnly)
* **CorsConfiguration**: [Cors](#cors)
* **CredentialsArn**: string (WriteOnly)
* **Description**: string
* **DisableExecuteApiEndpoint**: bool
* **DisableSchemaValidation**: bool (WriteOnly)
* **FailOnWarnings**: bool (WriteOnly)
* **Name**: string
* **ProtocolType**: string
* **RouteKey**: string (WriteOnly)
* **RouteSelectionExpression**: string
* **Tags**: [Api_Tags](#apitags): This resource type use map for Tags, suggest to use List of Tag
* **Target**: string (WriteOnly)
* **Version**: string

## Api_Body
### Properties

## BodyS3Location
### Properties
* **Bucket**: string (WriteOnly)
* **Etag**: string (WriteOnly)
* **Key**: string (WriteOnly)
* **Version**: string (WriteOnly)

## Cors
### Properties
* **AllowCredentials**: bool
* **AllowHeaders**: string[]
* **AllowMethods**: string[]
* **AllowOrigins**: string[]
* **ExposeHeaders**: string[]
* **MaxAge**: int

## Api_Tags
### Properties

## AWS.ApiGatewayV2/ModelProperties
### Properties
* **ApiId**: string (Required)
* **ContentType**: string
* **Description**: string
* **ModelId**: string (ReadOnly)
* **Name**: string (Required)
* **Schema**: [Model_Schema](#modelschema) (Required)

## Model_Schema
### Properties

## AWS.ApiGatewayV2/VpcLinkProperties
### Properties
* **Name**: string (Required)
* **SecurityGroupIds**: string[]
* **SubnetIds**: string[] (Required)
* **Tags**: [VpcLink_Tags](#vpclinktags): This resource type use map for Tags, suggest to use List of Tag
* **VpcLinkId**: string (ReadOnly)

## VpcLink_Tags
### Properties
