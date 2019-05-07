# ![LOGO](logo.png) ApiManagementClient **flow**ground Connector

## Description

A generated **flow**ground connector for the ApiManagementClient API (version 2018-06-01-preview).

Generated from: https://api.apis.guru/v2/specs/azure.com/apimanagement-apimsubscriptions/2018-06-01-preview/swagger.json<br/>
Generated at: 2019-05-07T17:37:11+03:00

## API Description

Use these REST APIs for performing operations on Subscription entity associated with your Azure API Management deployment. The Subscription entity represents the association between a user and a product in API Management. Products contain one or more APIs, and once a product is published, developers can subscribe to the product and begin to use the product’s APIs.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Lists all subscriptions of the API Management service instance.

*Tags:* `Subscription`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `serviceName` - _required_ - The name of the API Management service.
* `$filter` - _optional_ - | Field       | Supported operators    | Supported functions               |
|-------------|------------------------|-----------------------------------|

|name | ge, le, eq, ne, gt, lt | substringof, contains, startswith, endswith|
|displayName | ge, le, eq, ne, gt, lt | substringof, contains, startswith, endswith|
|stateComment | ge, le, eq, ne, gt, lt | substringof, contains, startswith, endswith|
|ownerId | ge, le, eq, ne, gt, lt | substringof, contains, startswith, endswith|
|scope | ge, le, eq, ne, gt, lt | substringof, contains, startswith, endswith|
|userId | ge, le, eq, ne, gt, lt | substringof, contains, startswith, endswith|
|productId | ge, le, eq, ne, gt, lt | substringof, contains, startswith, endswith|
|state | eq |    |
|user |     |    |

* `$top` - _optional_ - Number of records to return.
* `$skip` - _optional_ - Number of records to skip.
* `api-version` - _required_ - Version of the API to be used with the client request.
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.

### Deletes the specified subscription.

*Tags:* `Subscription`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `serviceName` - _required_ - The name of the API Management service.
* `sid` - _required_ - Subscription entity Identifier. The entity represents the association between a user and a product in API Management.
* `If-Match` - _required_ - ETag of the Entity. ETag should match the current entity state from the header response of the GET request or it should be * for unconditional update.
* `api-version` - _required_ - Version of the API to be used with the client request.
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.

### Gets the specified Subscription entity.

*Tags:* `Subscription`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `serviceName` - _required_ - The name of the API Management service.
* `sid` - _required_ - Subscription entity Identifier. The entity represents the association between a user and a product in API Management.
* `api-version` - _required_ - Version of the API to be used with the client request.
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.

### Gets the entity state (Etag) version of the apimanagement subscription specified by its identifier.

*Tags:* `Subscription`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `serviceName` - _required_ - The name of the API Management service.
* `sid` - _required_ - Subscription entity Identifier. The entity represents the association between a user and a product in API Management.
* `api-version` - _required_ - Version of the API to be used with the client request.
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.

### Updates the details of a subscription specified by its identifier.

*Tags:* `Subscription`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `serviceName` - _required_ - The name of the API Management service.
* `sid` - _required_ - Subscription entity Identifier. The entity represents the association between a user and a product in API Management.
* `notify` - _optional_ - Notify change in Subscription State. 
 - If false, do not send any email notification for change of state of subscription 
 - If true, send email notification of change of state of subscription 
* `If-Match` - _required_ - ETag of the Entity. ETag should match the current entity state from the header response of the GET request or it should be * for unconditional update.
* `api-version` - _required_ - Version of the API to be used with the client request.
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.

### Creates or updates the subscription of specified user to the specified product.

*Tags:* `Subscription`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `serviceName` - _required_ - The name of the API Management service.
* `sid` - _required_ - Subscription entity Identifier. The entity represents the association between a user and a product in API Management.
* `notify` - _optional_ - Notify change in Subscription State. 
 - If false, do not send any email notification for change of state of subscription 
 - If true, send email notification of change of state of subscription 
* `If-Match` - _optional_ - ETag of the Entity. Not required when creating an entity, but required when updating an entity.
* `api-version` - _required_ - Version of the API to be used with the client request.
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.

### Regenerates primary key of existing subscription of the API Management service instance.

*Tags:* `Subscriptions`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `serviceName` - _required_ - The name of the API Management service.
* `sid` - _required_ - Subscription entity Identifier. The entity represents the association between a user and a product in API Management.
* `api-version` - _required_ - Version of the API to be used with the client request.
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.

### Regenerates secondary key of existing subscription of the API Management service instance.

*Tags:* `Subscriptions`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `serviceName` - _required_ - The name of the API Management service.
* `sid` - _required_ - Subscription entity Identifier. The entity represents the association between a user and a product in API Management.
* `api-version` - _required_ - Version of the API to be used with the client request.
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.

## License

**flow**ground :- Telekom iPaaS / azure-com-apimanagement-apimsubscriptions-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
