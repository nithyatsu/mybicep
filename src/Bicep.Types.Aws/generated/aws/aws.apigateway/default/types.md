# AWS.ApiGateway @ default

## Resource AWS.ApiGateway/Account@default
* **Valid Scope(s)**: Unknown
### Properties
* **alias**: string (Required): the resource alias
* **name**: string: the resource name
* **properties**: [AWS.ApiGateway/AccountProperties](#awsapigatewayaccountproperties): properties of the resource

## Resource AWS.ApiGateway/ApiKey@default
* **Valid Scope(s)**: Unknown
### Properties
* **alias**: string (Required): the resource alias
* **name**: string: the resource name
* **properties**: [AWS.ApiGateway/ApiKeyProperties](#awsapigatewayapikeyproperties): properties of the resource

## Resource AWS.ApiGateway/Authorizer@default
* **Valid Scope(s)**: Unknown
### Properties
* **alias**: string (Required): the resource alias
* **name**: string: the resource name
* **properties**: [AWS.ApiGateway/AuthorizerProperties](#awsapigatewayauthorizerproperties) (Required): properties of the resource

## Resource AWS.ApiGateway/BasePathMapping@default
* **Valid Scope(s)**: Unknown
### Properties
* **alias**: string (Required): the resource alias
* **name**: string: the resource name
* **properties**: [AWS.ApiGateway/BasePathMappingProperties](#awsapigatewaybasepathmappingproperties) (Required): properties of the resource

## Resource AWS.ApiGateway/ClientCertificate@default
* **Valid Scope(s)**: Unknown
### Properties
* **alias**: string (Required): the resource alias
* **name**: string: the resource name
* **properties**: [AWS.ApiGateway/ClientCertificateProperties](#awsapigatewayclientcertificateproperties): properties of the resource

## Resource AWS.ApiGateway/Deployment@default
* **Valid Scope(s)**: Unknown
### Properties
* **alias**: string (Required): the resource alias
* **name**: string: the resource name
* **properties**: [AWS.ApiGateway/DeploymentProperties](#awsapigatewaydeploymentproperties) (Required): properties of the resource

## Resource AWS.ApiGateway/DocumentationPart@default
* **Valid Scope(s)**: Unknown
### Properties
* **alias**: string (Required): the resource alias
* **name**: string: the resource name
* **properties**: [AWS.ApiGateway/DocumentationPartProperties](#awsapigatewaydocumentationpartproperties) (Required): properties of the resource

## Resource AWS.ApiGateway/DocumentationVersion@default
* **Valid Scope(s)**: Unknown
### Properties
* **alias**: string (Required): the resource alias
* **name**: string: the resource name
* **properties**: [AWS.ApiGateway/DocumentationVersionProperties](#awsapigatewaydocumentationversionproperties) (Required): properties of the resource

## Resource AWS.ApiGateway/DomainName@default
* **Valid Scope(s)**: Unknown
### Properties
* **alias**: string (Required): the resource alias
* **name**: string: the resource name
* **properties**: [AWS.ApiGateway/DomainNameProperties](#awsapigatewaydomainnameproperties): properties of the resource

## Resource AWS.ApiGateway/Method@default
* **Valid Scope(s)**: Unknown
### Properties
* **alias**: string (Required): the resource alias
* **name**: string: the resource name
* **properties**: [AWS.ApiGateway/MethodProperties](#awsapigatewaymethodproperties) (Required): properties of the resource

## Resource AWS.ApiGateway/Model@default
* **Valid Scope(s)**: Unknown
### Properties
* **alias**: string (Required): the resource alias
* **name**: string: the resource name
* **properties**: [AWS.ApiGateway/ModelProperties](#awsapigatewaymodelproperties) (Required): properties of the resource

## Resource AWS.ApiGateway/RequestValidator@default
* **Valid Scope(s)**: Unknown
### Properties
* **alias**: string (Required): the resource alias
* **name**: string: the resource name
* **properties**: [AWS.ApiGateway/RequestValidatorProperties](#awsapigatewayrequestvalidatorproperties) (Required): properties of the resource

## Resource AWS.ApiGateway/Resource@default
* **Valid Scope(s)**: Unknown
### Properties
* **alias**: string (Required): the resource alias
* **name**: string: the resource name
* **properties**: [AWS.ApiGateway/ResourceProperties](#awsapigatewayresourceproperties) (Required): properties of the resource

## Resource AWS.ApiGateway/RestApi@default
* **Valid Scope(s)**: Unknown
### Properties
* **alias**: string (Required): the resource alias
* **name**: string: the resource name
* **properties**: [AWS.ApiGateway/RestApiProperties](#awsapigatewayrestapiproperties): properties of the resource

## Resource AWS.ApiGateway/Stage@default
* **Valid Scope(s)**: Unknown
### Properties
* **alias**: string (Required): the resource alias
* **name**: string: the resource name
* **properties**: [AWS.ApiGateway/StageProperties](#awsapigatewaystageproperties) (Required): properties of the resource

## Resource AWS.ApiGateway/UsagePlan@default
* **Valid Scope(s)**: Unknown
### Properties
* **alias**: string (Required): the resource alias
* **name**: string: the resource name
* **properties**: [AWS.ApiGateway/UsagePlanProperties](#awsapigatewayusageplanproperties): properties of the resource

## Resource AWS.ApiGateway/VpcLink@default
* **Valid Scope(s)**: Unknown
### Properties
* **alias**: string (Required): the resource alias
* **name**: string: the resource name
* **properties**: [AWS.ApiGateway/VpcLinkProperties](#awsapigatewayvpclinkproperties) (Required): properties of the resource

## AWS.ApiGateway/AccountProperties
### Properties
* **CloudWatchRoleArn**: string: The Amazon Resource Name (ARN) of an IAM role that has write access to CloudWatch Logs in your account.
* **Id**: string (ReadOnly, Identifier): Primary identifier which is manually generated.

## AWS.ApiGateway/ApiKeyProperties
### Properties
* **APIKeyId**: string (ReadOnly, Identifier): A Unique Key ID which identifies the API Key. Generated by the Create API and returned by the Read and List APIs 
* **CustomerId**: string: An AWS Marketplace customer identifier to use when integrating with the AWS SaaS Marketplace.
* **Description**: string: A description of the purpose of the API key.
* **Enabled**: bool: Indicates whether the API key can be used by clients.
* **GenerateDistinctId**: bool (WriteOnly): Specifies whether the key identifier is distinct from the created API key value. This parameter is deprecated and should not be used.
* **Name**: string: A name for the API key. If you don't specify a name, AWS CloudFormation generates a unique physical ID and uses that ID for the API key name.
* **StageKeys**: [StageKey](#stagekey)[]: A list of stages to associate with this API key.
* **Tags**: [Tag](#tag)[]: An array of arbitrary tags (key-value pairs) to associate with the API key.
* **Value**: string: The value of the API key. Must be at least 20 characters long.

## StageKey
### Properties
* **RestApiId**: string: The ID of a RestApi resource that includes the stage with which you want to associate the API key.
* **StageName**: string: The name of the stage with which to associate the API key. The stage must be included in the RestApi resource that you specified in the RestApiId property. 

## Tag
### Properties
* **Key**: string (Required): The key name of the tag. You can specify a value that is 1 to 128 Unicode characters in length and cannot be prefixed with aws:. You can use any of the following characters: the set of Unicode letters, digits, whitespace, _, ., /, =, +, and -.
* **Value**: string (Required): The value for the tag. You can specify a value that is 0 to 256 Unicode characters in length and cannot be prefixed with aws:. You can use any of the following characters: the set of Unicode letters, digits, whitespace, _, ., /, =, +, and -. 

## AWS.ApiGateway/AuthorizerProperties
### Properties
* **AuthorizerCredentials**: string: Specifies the required credentials as an IAM role for API Gateway to invoke the authorizer.
* **AuthorizerId**: string (ReadOnly, Identifier)
* **AuthorizerResultTtlInSeconds**: int: The TTL in seconds of cached authorizer results.
* **AuthorizerUri**: string: Specifies the authorizer's Uniform Resource Identifier (URI).
* **AuthType**: string: Optional customer-defined field, used in OpenAPI imports and exports without functional impact.
* **IdentitySource**: string: The identity source for which authorization is requested.
* **IdentityValidationExpression**: string: A validation expression for the incoming identity token.
* **Name**: string (Required): The name of the authorizer.
* **ProviderARNs**: string[]: A list of the Amazon Cognito user pool ARNs for the COGNITO_USER_POOLS authorizer.
* **RestApiId**: string (Required, Identifier): The identifier of the API.
* **Type**: string (Required): The authorizer type.

## AWS.ApiGateway/BasePathMappingProperties
### Properties
* **BasePath**: string (Identifier): The base path name that callers of the API must provide in the URL after the domain name.
* **DomainName**: string (Required, Identifier): The DomainName of an AWS::ApiGateway::DomainName resource.
* **RestApiId**: string: The ID of the API.
* **Stage**: string: The name of the API's stage.

## AWS.ApiGateway/ClientCertificateProperties
### Properties
* **ClientCertificateId**: string (ReadOnly, Identifier): The Primary Identifier of the Client Certficate, generated by a Create API Call
* **Description**: string: A description of the client certificate.
* **Tags**: [Tag](#tag)[]: An array of arbitrary tags (key-value pairs) to associate with the client certificate.

## Tag
### Properties
* **Key**: string (Required)
* **Value**: string (Required)

## AWS.ApiGateway/DeploymentProperties
### Properties
* **DeploymentCanarySettings**: [DeploymentCanarySettings](#deploymentcanarysettings) (WriteOnly): Specifies settings for the canary deployment.
* **DeploymentId**: string (ReadOnly, Identifier): Primary Id for this resource
* **Description**: string: A description of the purpose of the API Gateway deployment.
* **RestApiId**: string (Required, Identifier): The ID of the RestApi resource to deploy. 
* **StageDescription**: [StageDescription](#stagedescription) (WriteOnly): Configures the stage that API Gateway creates with this deployment.
* **StageName**: string (WriteOnly): A name for the stage that API Gateway creates with this deployment. Use only alphanumeric characters.

## DeploymentCanarySettings
### Properties
* **PercentTraffic**: int: The percentage (0-100) of traffic diverted to a canary deployment.
* **StageVariableOverrides**: [Deployment_StageVariableOverrides](#deploymentstagevariableoverrides): Stage variables overridden for a canary release deployment, including new stage variables introduced in the canary. These stage variables are represented as a string-to-string map between stage variable names and their values. Duplicates are not allowed.
* **UseStageCache**: bool: Whether the canary deployment uses the stage cache.

## Deployment_StageVariableOverrides
### Properties

## StageDescription
### Properties
* **AccessLogSetting**: [AccessLogSetting](#accesslogsetting): Specifies settings for logging access in this stage.
* **CacheClusterEnabled**: bool: Indicates whether cache clustering is enabled for the stage.
* **CacheClusterSize**: string: The size of the stage's cache cluster.
* **CacheDataEncrypted**: bool: The time-to-live (TTL) period, in seconds, that specifies how long API Gateway caches responses. 
* **CacheTtlInSeconds**: int: The time-to-live (TTL) period, in seconds, that specifies how long API Gateway caches responses. 
* **CachingEnabled**: bool: Indicates whether responses are cached and returned for requests. You must enable a cache cluster on the stage to cache responses.
* **CanarySetting**: [CanarySetting](#canarysetting): Specifies settings for the canary deployment in this stage.
* **ClientCertificateId**: string: The identifier of the client certificate that API Gateway uses to call your integration endpoints in the stage. 
* **DataTraceEnabled**: bool: Indicates whether data trace logging is enabled for methods in the stage. API Gateway pushes these logs to Amazon CloudWatch Logs. 
* **Description**: string: A description of the purpose of the stage.
* **DocumentationVersion**: string: The version identifier of the API documentation snapshot.
* **LoggingLevel**: string: The logging level for this method. For valid values, see the loggingLevel property of the Stage resource in the Amazon API Gateway API Reference. 
* **MethodSettings**: [MethodSetting](#methodsetting)[]: Configures settings for all of the stage's methods.
* **MetricsEnabled**: bool: Indicates whether Amazon CloudWatch metrics are enabled for methods in the stage.
* **Tags**: [Tag](#tag)[]: An array of arbitrary tags (key-value pairs) to associate with the stage.
* **ThrottlingBurstLimit**: int: The number of burst requests per second that API Gateway permits across all APIs, stages, and methods in your AWS account.
* **ThrottlingRateLimit**: int: The number of steady-state requests per second that API Gateway permits across all APIs, stages, and methods in your AWS account.
* **TracingEnabled**: bool: Specifies whether active tracing with X-ray is enabled for this stage.
* **Variables**: [Deployment_Variables](#deploymentvariables): A map that defines the stage variables. Variable names must consist of alphanumeric characters, and the values must match the following regular expression: [A-Za-z0-9-._~:/?#&=,]+. 

## AccessLogSetting
### Properties
* **DestinationArn**: string: The Amazon Resource Name (ARN) of the CloudWatch Logs log group or Kinesis Data Firehose delivery stream to receive access logs. If you specify a Kinesis Data Firehose delivery stream, the stream name must begin with amazon-apigateway-. 
* **Format**: string: A single line format of the access logs of data, as specified by selected $context variables. The format must include at least $context.requestId. 

## CanarySetting
### Properties
* **PercentTraffic**: int: The percent (0-100) of traffic diverted to a canary deployment.
* **StageVariableOverrides**: [Deployment_StageVariableOverrides](#deploymentstagevariableoverrides): Stage variables overridden for a canary release deployment, including new stage variables introduced in the canary. These stage variables are represented as a string-to-string map between stage variable names and their values. 
* **UseStageCache**: bool: Whether the canary deployment uses the stage cache or not.

## Deployment_StageVariableOverrides
### Properties

## MethodSetting
### Properties
* **CacheDataEncrypted**: bool: Indicates whether the cached responses are encrypted
* **CacheTtlInSeconds**: int: The time-to-live (TTL) period, in seconds, that specifies how long API Gateway caches responses. 
* **CachingEnabled**: bool: Indicates whether responses are cached and returned for requests. You must enable a cache cluster on the stage to cache responses.
* **DataTraceEnabled**: bool: Indicates whether data trace logging is enabled for methods in the stage. API Gateway pushes these logs to Amazon CloudWatch Logs. 
* **HttpMethod**: string: The HTTP method.
* **LoggingLevel**: string: The logging level for this method. For valid values, see the loggingLevel property of the Stage resource in the Amazon API Gateway API Reference. 
* **MetricsEnabled**: bool: Indicates whether Amazon CloudWatch metrics are enabled for methods in the stage.
* **ResourcePath**: string: The resource path for this method. Forward slashes (/) are encoded as ~1 and the initial slash must include a forward slash. 
* **ThrottlingBurstLimit**: int: The number of burst requests per second that API Gateway permits across all APIs, stages, and methods in your AWS account.
* **ThrottlingRateLimit**: int: The number of steady-state requests per second that API Gateway permits across all APIs, stages, and methods in your AWS account.

## Tag
### Properties
* **Key**: string (Required): The key name of the tag
* **Value**: string (Required): The value for the tag

## Deployment_Variables
### Properties

## AWS.ApiGateway/DocumentationPartProperties
### Properties
* **DocumentationPartId**: string (ReadOnly, Identifier): The identifier of the documentation Part.
* **Location**: [Location](#location) (Required): The location of the API entity that the documentation applies to.
* **Properties**: string (Required): The documentation content map of the targeted API entity.
* **RestApiId**: string (Required, Identifier): Identifier of the targeted API entity

## Location
### Properties
* **Method**: string: The HTTP verb of a method.
* **Name**: string: The name of the targeted API entity.
* **Path**: string: The URL path of the target.
* **StatusCode**: string: The HTTP status code of a response.
* **Type**: string: The type of API entity that the documentation content applies to.

## AWS.ApiGateway/DocumentationVersionProperties
### Properties
* **Description**: string: The description of the API documentation snapshot.
* **DocumentationVersion**: string (Required, Identifier): The version identifier of the API documentation snapshot.
* **RestApiId**: string (Required, Identifier): The identifier of the API.

## AWS.ApiGateway/DomainNameProperties
### Properties
* **CertificateArn**: string
* **DistributionDomainName**: string (ReadOnly)
* **DistributionHostedZoneId**: string (ReadOnly)
* **DomainName**: string (Identifier)
* **EndpointConfiguration**: [EndpointConfiguration](#endpointconfiguration)
* **MutualTlsAuthentication**: [MutualTlsAuthentication](#mutualtlsauthentication)
* **OwnershipVerificationCertificateArn**: string
* **RegionalCertificateArn**: string
* **RegionalDomainName**: string (ReadOnly)
* **RegionalHostedZoneId**: string (ReadOnly)
* **SecurityPolicy**: string
* **Tags**: [Tag](#tag)[]

## EndpointConfiguration
### Properties
* **Types**: string[]

## MutualTlsAuthentication
### Properties
* **TruststoreUri**: string
* **TruststoreVersion**: string

## Tag
### Properties
* **Key**: string
* **Value**: string

## AWS.ApiGateway/MethodProperties
### Properties
* **ApiKeyRequired**: bool: Indicates whether the method requires clients to submit a valid API key.
* **AuthorizationScopes**: string[]: A list of authorization scopes configured on the method.
* **AuthorizationType**: string: The method's authorization type.
* **AuthorizerId**: string: The identifier of the authorizer to use on this method.
* **HttpMethod**: string (Required, Identifier): The backend system that the method calls when it receives a request.
* **Integration**: [Integration](#integration): The backend system that the method calls when it receives a request.
* **MethodResponses**: [MethodResponse](#methodresponse)[]: The responses that can be sent to the client who calls the method.
* **OperationName**: string: A friendly operation name for the method.
* **RequestModels**: [Method_RequestModels](#methodrequestmodels): The resources that are used for the request's content type. Specify request models as key-value pairs (string-to-string mapping), with a content type as the key and a Model resource name as the value.
* **RequestParameters**: [Method_RequestParameters](#methodrequestparameters): The request parameters that API Gateway accepts. Specify request parameters as key-value pairs (string-to-Boolean mapping), with a source as the key and a Boolean as the value.
* **RequestValidatorId**: string: The ID of the associated request validator.
* **ResourceId**: string (Required, Identifier): The ID of an API Gateway resource.
* **RestApiId**: string (Required, Identifier): The ID of the RestApi resource in which API Gateway creates the method.

## Integration
### Properties
* **CacheKeyParameters**: string[]: A list of request parameters whose values API Gateway caches.
* **CacheNamespace**: string: An API-specific tag group of related cached parameters.
* **ConnectionId**: string: The ID of the VpcLink used for the integration when connectionType=VPC_LINK, otherwise undefined.
* **ConnectionType**: string: The type of the network connection to the integration endpoint.
* **ContentHandling**: string: Specifies how to handle request payload content type conversions.
* **Credentials**: string: The credentials that are required for the integration.
* **IntegrationHttpMethod**: string: The integration's HTTP method type.
* **IntegrationResponses**: [IntegrationResponse](#integrationresponse)[]: The response that API Gateway provides after a method's backend completes processing a request.
* **PassthroughBehavior**: string: Indicates when API Gateway passes requests to the targeted backend.
* **RequestParameters**: [Method_RequestParameters](#methodrequestparameters): The request parameters that API Gateway sends with the backend request.
* **RequestTemplates**: [Method_RequestTemplates](#methodrequesttemplates): A map of Apache Velocity templates that are applied on the request payload.
* **TimeoutInMillis**: int: Custom timeout between 50 and 29,000 milliseconds.
* **Type**: string (Required): The type of backend that your method is running.
* **Uri**: string: The Uniform Resource Identifier (URI) for the integration.

## IntegrationResponse
### Properties
* **ContentHandling**: string: Specifies how to handle request payload content type conversions.
* **ResponseParameters**: [Method_ResponseParameters](#methodresponseparameters): The response parameters from the backend response that API Gateway sends to the method response.
* **ResponseTemplates**: [Method_ResponseTemplates](#methodresponsetemplates): The templates that are used to transform the integration response body. Specify templates as key-value pairs (string-to-string mappings), with a content type as the key and a template as the value.
* **SelectionPattern**: string: A regular expression that specifies which error strings or status codes from the backend map to the integration response.
* **StatusCode**: string (Required): The status code that API Gateway uses to map the integration response to a MethodResponse status code.

## Method_ResponseParameters
### Properties

## Method_ResponseTemplates
### Properties

## Method_RequestParameters
### Properties

## Method_RequestTemplates
### Properties

## MethodResponse
### Properties
* **ResponseModels**: [Method_ResponseModels](#methodresponsemodels): The resources used for the response's content type. Specify response models as key-value pairs (string-to-string maps), with a content type as the key and a Model resource name as the value.
* **ResponseParameters**: [Method_ResponseParameters](#methodresponseparameters): Response parameters that API Gateway sends to the client that called a method. Specify response parameters as key-value pairs (string-to-Boolean maps), with a destination as the key and a Boolean as the value.
* **StatusCode**: string (Required): The method response's status code, which you map to an IntegrationResponse.

## Method_ResponseModels
### Properties

## Method_ResponseParameters
### Properties

## Method_RequestModels
### Properties

## Method_RequestParameters
### Properties

## AWS.ApiGateway/ModelProperties
### Properties
* **ContentType**: string: The content type for the model.
* **Description**: string: A description that identifies this model.
* **Name**: string (Identifier): A name for the model. If you don't specify a name, AWS CloudFormation generates a unique physical ID and uses that ID for the model name.
* **RestApiId**: string (Required, Identifier): The ID of a REST API with which to associate this model.
* **Schema**: [Model_Schema](#modelschema) | string: The schema to use to transform data to one or more output formats. Specify null ({}) if you don't want to specify a schema.

## AWS.ApiGateway/RequestValidatorProperties
### Properties
* **Name**: string: Name of the request validator.
* **RequestValidatorId**: string (ReadOnly, Identifier): ID of the request validator.
* **RestApiId**: string (Required, Identifier): The identifier of the targeted API entity.
* **ValidateRequestBody**: bool: Indicates whether to validate the request body according to the configured schema for the targeted API and method. 
* **ValidateRequestParameters**: bool: Indicates whether to validate request parameters.

## AWS.ApiGateway/ResourceProperties
### Properties
* **ParentId**: string (Required): The parent resource's identifier.
* **PathPart**: string (Required): The last path segment for this resource.
* **ResourceId**: string (ReadOnly, Identifier): A unique primary identifier for a Resource
* **RestApiId**: string (Required, Identifier): The ID of the RestApi resource in which you want to create this resource..

## AWS.ApiGateway/RestApiProperties
### Properties
* **ApiKeySourceType**: string
* **BinaryMediaTypes**: string[]
* **Body**: [RestApi_Body](#restapibody) | string (WriteOnly)
* **BodyS3Location**: [S3Location](#s3location) (WriteOnly)
* **CloneFrom**: string (WriteOnly)
* **Description**: string
* **DisableExecuteApiEndpoint**: bool
* **EndpointConfiguration**: [EndpointConfiguration](#endpointconfiguration)
* **FailOnWarnings**: bool (WriteOnly)
* **MinimumCompressionSize**: int
* **Mode**: string (WriteOnly)
* **Name**: string
* **Parameters**: [RestApi_Parameters](#restapiparameters) | string (WriteOnly)
* **Policy**: [RestApi_Policy](#restapipolicy) | string
* **RestApiId**: string (ReadOnly, Identifier)
* **RootResourceId**: string (ReadOnly)
* **Tags**: [Tag](#tag)[]

## S3Location
### Properties
* **Bucket**: string
* **ETag**: string
* **Key**: string
* **Version**: string

## EndpointConfiguration
### Properties
* **Types**: string[]
* **VpcEndpointIds**: string[]

## Tag
### Properties
* **Key**: string (Required)
* **Value**: string (Required)

## AWS.ApiGateway/StageProperties
### Properties
* **AccessLogSetting**: [AccessLogSetting](#accesslogsetting): Specifies settings for logging access in this stage.
* **CacheClusterEnabled**: bool: Indicates whether cache clustering is enabled for the stage.
* **CacheClusterSize**: string: The stage's cache cluster size.
* **CanarySetting**: [CanarySetting](#canarysetting): Specifies settings for the canary deployment in this stage.
* **ClientCertificateId**: string: The ID of the client certificate that API Gateway uses to call your integration endpoints in the stage. 
* **DeploymentId**: string: The ID of the deployment that the stage is associated with. This parameter is required to create a stage. 
* **Description**: string: A description of the stage.
* **DocumentationVersion**: string: The version ID of the API documentation snapshot.
* **MethodSettings**: [MethodSetting](#methodsetting)[]: Settings for all methods in the stage.
* **RestApiId**: string (Required, Identifier): The ID of the RestApi resource that you're deploying with this stage.
* **StageName**: string (Identifier): The name of the stage, which API Gateway uses as the first path segment in the invoked Uniform Resource Identifier (URI).
* **Tags**: [Tag](#tag)[]: An array of arbitrary tags (key-value pairs) to associate with the stage.
* **TracingEnabled**: bool: Specifies whether active X-Ray tracing is enabled for this stage.
* **Variables**: [Stage_Variables](#stagevariables): A map (string-to-string map) that defines the stage variables, where the variable name is the key and the variable value is the value.

## AccessLogSetting
### Properties
* **DestinationArn**: string: The Amazon Resource Name (ARN) of the CloudWatch Logs log group or Kinesis Data Firehose delivery stream to receive access logs. If you specify a Kinesis Data Firehose delivery stream, the stream name must begin with amazon-apigateway-. This parameter is required to enable access logging.
* **Format**: string: A single line format of the access logs of data, as specified by selected $context variables (https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-mapping-template-reference.html#context-variable-reference). The format must include at least $context.requestId. This parameter is required to enable access logging.

## CanarySetting
### Properties
* **DeploymentId**: string: The identifier of the deployment that the stage points to.
* **PercentTraffic**: int: The percentage (0-100) of traffic diverted to a canary deployment.
* **StageVariableOverrides**: [Stage_StageVariableOverrides](#stagestagevariableoverrides): Stage variables overridden for a canary release deployment, including new stage variables introduced in the canary. These stage variables are represented as a string-to-string map between stage variable names and their values.
* **UseStageCache**: bool: Whether the canary deployment uses the stage cache or not.

## Stage_StageVariableOverrides
### Properties

## MethodSetting
### Properties
* **CacheDataEncrypted**: bool: Indicates whether the cached responses are encrypted.
* **CacheTtlInSeconds**: int: The time-to-live (TTL) period, in seconds, that specifies how long API Gateway caches responses.
* **CachingEnabled**: bool: Indicates whether responses are cached and returned for requests. You must enable a cache cluster on the stage to cache responses.
* **DataTraceEnabled**: bool: Indicates whether data trace logging is enabled for methods in the stage. API Gateway pushes these logs to Amazon CloudWatch Logs.
* **HttpMethod**: string: The HTTP method. You can use an asterisk (*) as a wildcard to apply method settings to multiple methods.
* **LoggingLevel**: string: The logging level for this method. For valid values, see the loggingLevel property of the Stage (https://docs.aws.amazon.com/apigateway/api-reference/resource/stage/#loggingLevel) resource in the Amazon API Gateway API Reference.
* **MetricsEnabled**: bool: Indicates whether Amazon CloudWatch metrics are enabled for methods in the stage.
* **ResourcePath**: string: The resource path for this method. Forward slashes (/) are encoded as ~1 and the initial slash must include a forward slash. For example, the path value /resource/subresource must be encoded as /~1resource~1subresource. To specify the root path, use only a slash (/). You can use an asterisk (*) as a wildcard to apply method settings to multiple methods.
* **ThrottlingBurstLimit**: int: The number of burst requests per second that API Gateway permits across all APIs, stages, and methods in your AWS account.
* **ThrottlingRateLimit**: int: The number of steady-state requests per second that API Gateway permits across all APIs, stages, and methods in your AWS account.

## Tag
### Properties
* **Key**: string (Required): The key name of the tag. You can specify a value that is 1 to 128 Unicode characters in length and cannot be prefixed with aws:.
* **Value**: string (Required): The value for the tag. You can specify a value that is 0 to 256 Unicode characters in length and cannot be prefixed with aws:.

## Stage_Variables
### Properties

## AWS.ApiGateway/UsagePlanProperties
### Properties
* **ApiStages**: [ApiStage](#apistage)[]: The API stages to associate with this usage plan.
* **Description**: string: A description of the usage plan.
* **Id**: string (ReadOnly, Identifier): The provider-assigned unique ID for this managed resource.
* **Quota**: [QuotaSettings](#quotasettings): Configures the number of requests that users can make within a given interval.
* **Tags**: [Tag](#tag)[]: An array of arbitrary tags (key-value pairs) to associate with the usage plan.
* **Throttle**: [ThrottleSettings](#throttlesettings): Configures the overall request rate (average requests per second) and burst capacity.
* **UsagePlanName**: string: A name for the usage plan.

## ApiStage
### Properties
* **ApiId**: string: The ID of an API that is in the specified Stage property that you want to associate with the usage plan.
* **Stage**: string: The name of the stage to associate with the usage plan.
* **Throttle**: [UsagePlan_Throttle](#usageplanthrottle): Map containing method-level throttling information for an API stage in a usage plan. The key for the map is the path and method for which to configure custom throttling, for example, '/pets/GET'. Duplicates are not allowed.

## UsagePlan_Throttle
### Properties

## QuotaSettings
### Properties
* **Limit**: int: The maximum number of requests that users can make within the specified time period.
* **Offset**: int: For the initial time period, the number of requests to subtract from the specified limit. When you first implement a usage plan, the plan might start in the middle of the week or month. With this property, you can decrease the limit for this initial time period.
* **Period**: string: The time period for which the maximum limit of requests applies, such as DAY or WEEK. For valid values, see the period property for the UsagePlan resource in the Amazon API Gateway REST API Reference.

## Tag
### Properties
* **Key**: string (Required): The key name of the tag. You can specify a value that is 1 to 128 Unicode characters in length and cannot be prefixed with aws:. You can use any of the following characters: the set of Unicode letters, digits, whitespace, _, ., /, =, +, and -.
* **Value**: string (Required): The value for the tag. You can specify a value that is 0 to 256 Unicode characters in length and cannot be prefixed with aws:. You can use any of the following characters: the set of Unicode letters, digits, whitespace, _, ., /, =, +, and -.

## ThrottleSettings
### Properties
* **BurstLimit**: int: The maximum API request rate limit over a time ranging from one to a few seconds. The maximum API request rate limit depends on whether the underlying token bucket is at its full capacity.
* **RateLimit**: int: The API request steady-state rate limit (average requests per second over an extended period of time).

## AWS.ApiGateway/VpcLinkProperties
### Properties
* **Description**: string: A description of the VPC link.
* **Name**: string (Required): A name for the VPC link.
* **Tags**: [Tag](#tag)[]: An array of arbitrary tags (key-value pairs) to associate with the stage.
* **TargetArns**: string[] (Required): The ARN of network load balancer of the VPC targeted by the VPC link. The network load balancer must be owned by the same AWS account of the API owner.
* **VpcLinkId**: string (ReadOnly, Identifier): The ID of the instance that backs VPC link.

## Tag
### Properties
* **Key**: string (Required)
* **Value**: string (Required)

