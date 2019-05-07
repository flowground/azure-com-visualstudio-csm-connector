# ![LOGO](logo.png) Visual Studio Resource Provider Client **flow**ground Connector

## Description

A generated **flow**ground connector for the Visual Studio Resource Provider Client API (version 2017-11-01-preview).

Generated from: https://api.apis.guru/v2/specs/azure.com/visualstudio-Csm/2017-11-01-preview/swagger.json<br/>
Generated at: 2019-05-07T17:39:20+03:00

## API Description

Use these APIs to manage Visual Studio Team Services resources through the Azure Resource Manager. All task operations conform to the HTTP/1.1 protocol specification and each operation returns an x-ms-request-id header that can be used to obtain information about the request. You must make sure that requests made to these resources are secure. For more information, see https://docs.microsoft.com/en-us/rest/api/index.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Operations_List

> Gets the details of all operations possible on the Microsoft.VisualStudio resource provider.

*Tags:* `Operations`

### Accounts_CheckNameAvailability

> Checks if the specified Visual Studio Team Services account name is available. Resource name can be either an account name or an account name and PUID.

*Tags:* `Accounts`

#### Input Parameters
* `subscriptionId` - _required_ - The Azure subscription identifier.
* `api-version` - _required_ - API Version

### Projects_ListByAccountResource

> Gets all Visual Studio Team Services project resources created in the specified Team Services account.

*Tags:* `Projects`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group within the Azure subscription.
* `subscriptionId` - _required_ - The Azure subscription identifier.
* `api-version` - _required_ - API Version
* `rootResourceName` - _required_ - Name of the Team Services account.

### Projects_Get

> Gets the details of a Team Services project resource.

*Tags:* `Projects`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group within the Azure subscription.
* `subscriptionId` - _required_ - The Azure subscription identifier.
* `api-version` - _required_ - API Version
* `rootResourceName` - _required_ - Name of the Team Services account.
* `resourceName` - _required_ - Name of the Team Services project.

### Projects_Update

> Updates the tags of the specified Team Services project.

*Tags:* `Projects`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group within the Azure subscription.
* `subscriptionId` - _required_ - The Azure subscription identifier.
* `api-version` - _required_ - API Version
* `rootResourceName` - _required_ - Name of the Team Services account.
* `resourceName` - _required_ - Name of the Team Services project.

### Projects_Create

> Creates a Team Services project in the collection with the specified name. 'VersionControlOption' and 'ProcessTemplateId' must be specified in the resource properties. Valid values for VersionControlOption: Git, Tfvc. Valid values for ProcessTemplateId: 6B724908-EF14-45CF-84F8-768B5384DA45, ADCC42AB-9882-485E-A3ED-7678F01F66BC, 27450541-8E31-4150-9947-DC59F998FC01 (these IDs correspond to Scrum, Agile, and CMMI process templates).

*Tags:* `Projects`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group within the Azure subscription.
* `subscriptionId` - _required_ - The Azure subscription identifier.
* `api-version` - _required_ - API Version
* `rootResourceName` - _required_ - Name of the Team Services account.
* `resourceName` - _required_ - Name of the Team Services project.
* `validating` - _optional_ - This parameter is ignored and should be set to an empty string.

### Accounts_ListByResourceGroup

> Gets all Visual Studio Team Services account resources under the resource group linked to the specified Azure subscription.

*Tags:* `Accounts`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group within the Azure subscription.
* `subscriptionId` - _required_ - The Azure subscription identifier.
* `api-version` - _required_ - API Version

### Extensions_ListByAccount

> Gets the details of the extension resources created within the resource group.

*Tags:* `Extensions`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group within the Azure subscription.
* `subscriptionId` - _required_ - The Azure subscription identifier.
* `api-version` - _required_ - API Version
* `accountResourceName` - _required_ - The name of the Visual Studio Team Services account resource.

### Extensions_Delete

> Removes an extension resource registration for a Visual Studio Team Services account.

*Tags:* `Extensions`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group within the Azure subscription.
* `subscriptionId` - _required_ - The Azure subscription identifier.
* `api-version` - _required_ - API Version
* `accountResourceName` - _required_ - The name of the Visual Studio Team Services account resource.
* `extensionResourceName` - _required_ - The name of the extension.

### Extensions_Get

> Gets the details of an extension associated with a Visual Studio Team Services account resource.

*Tags:* `Extensions`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group within the Azure subscription.
* `subscriptionId` - _required_ - The Azure subscription identifier.
* `api-version` - _required_ - API Version
* `accountResourceName` - _required_ - The name of the Visual Studio Team Services account resource.
* `extensionResourceName` - _required_ - The name of the extension.

### Extensions_Update

> Updates an existing extension registration for the Visual Studio Team Services account.

*Tags:* `Extensions`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group within the Azure subscription.
* `subscriptionId` - _required_ - The Azure subscription identifier.
* `api-version` - _required_ - API Version
* `accountResourceName` - _required_ - The name of the Visual Studio Team Services account resource.
* `extensionResourceName` - _required_ - The name of the extension.

### Extensions_Create

> Registers the extension with a Visual Studio Team Services account.

*Tags:* `Extensions`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group within the Azure subscription.
* `subscriptionId` - _required_ - The Azure subscription identifier.
* `api-version` - _required_ - API Version
* `accountResourceName` - _required_ - The name of the Visual Studio Team Services account resource.
* `extensionResourceName` - _required_ - The name of the extension.

### Accounts_Delete

> Deletes a Visual Studio Team Services account resource.

*Tags:* `Accounts`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group within the Azure subscription.
* `subscriptionId` - _required_ - The Azure subscription identifier.
* `api-version` - _required_ - API Version
* `resourceName` - _required_ - Name of the resource.

### Accounts_Get

> Gets the Visual Studio Team Services account resource details.

*Tags:* `Accounts`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group within the Azure subscription.
* `subscriptionId` - _required_ - The Azure subscription identifier.
* `api-version` - _required_ - API Version
* `resourceName` - _required_ - Name of the resource.

### Accounts_CreateOrUpdate

> Creates or updates a Visual Studio Team Services account resource.

*Tags:* `Accounts`

#### Input Parameters
* `resourceGroupName` - _required_ - Name of the resource group within the Azure subscription.
* `subscriptionId` - _required_ - The Azure subscription identifier.
* `api-version` - _required_ - API Version
* `resourceName` - _required_ - Name of the resource.

## License

**flow**ground :- Telekom iPaaS / azure-com-visualstudio-csm-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
