---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectorGroup = new ConnectorGroup
{
	Name = "name-value",
	IsDefault = false
};

await graphClient.OnPremisesPublishingProfiles["applicationProxy"].ConnectorGroups
	.Request()
	.AddAsync(connectorGroup);

```