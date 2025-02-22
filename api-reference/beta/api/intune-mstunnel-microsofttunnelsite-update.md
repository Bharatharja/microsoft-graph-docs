---
title: "Update microsoftTunnelSite"
description: "Update the properties of a microsoftTunnelSite object."
author: "dougeby"
localization_priority: Normal
ms.prod: "intune"
doc_type: apiPageType
---

# Update microsoftTunnelSite

Namespace: microsoft.graph

> **Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Update the properties of a [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) object.

## Prerequisites
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|DeviceManagementConfiguration.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|DeviceManagementConfiguration.ReadWrite.All|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer &lt;token&gt; Required.|
|Accept|application/json|

## Request body
In the request body, supply a JSON representation for the [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) object.

The following table shows the properties that are required when you create the [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|The MicrosoftTunnelSite's Id|
|displayName|String|The MicrosoftTunnelSite's display name|
|description|String|The MicrosoftTunnelSite's description|
|publicAddress|String|The MicrosoftTunnelSite's public domain name or IP address|
|upgradeWindowUtcOffsetInMinutes|Int32|The site's timezone represented as a minute offset from UTC|
|upgradeWindowStartTime|TimeOfDay|The site's upgrade window start time of day|
|upgradeWindowEndTime|TimeOfDay|The site's upgrade window end time of day|
|upgradeAutomatically|Boolean|The site's automatic upgrade setting. True for automatic upgrades, false for manual control|
|upgradeAvailable|Boolean|True if an upgrade is available|
|internalNetworkProbeUrl|String|The MicrosoftTunnelSite's Internal Network Access Probe URL|
|enableCertificatePinning|Boolean|When set to true, certificate pinning will be enforced on connections between the Microsoft Tunnel server and Microsoft Tunnel clients. When set to false, certificate pinning will be disabled.|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance.|



## Response
If successful, this method returns a `200 OK` response code and an updated [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) object in the response body.

## Example

### Request
Here is an example of the request.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}
Content-type: application/json
Content-length: 561

{
  "@odata.type": "#microsoft.graph.microsoftTunnelSite",
  "displayName": "Display Name value",
  "description": "Description value",
  "publicAddress": "Public Address value",
  "upgradeWindowUtcOffsetInMinutes": 15,
  "upgradeWindowStartTime": "12:01:27.3030000",
  "upgradeWindowEndTime": "11:57:17.9830000",
  "upgradeAutomatically": true,
  "upgradeAvailable": true,
  "internalNetworkProbeUrl": "https://example.com/internalNetworkProbeUrl/",
  "enableCertificatePinning": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 610

{
  "@odata.type": "#microsoft.graph.microsoftTunnelSite",
  "id": "b2f7dc3e-dc3e-b2f7-3edc-f7b23edcf7b2",
  "displayName": "Display Name value",
  "description": "Description value",
  "publicAddress": "Public Address value",
  "upgradeWindowUtcOffsetInMinutes": 15,
  "upgradeWindowStartTime": "12:01:27.3030000",
  "upgradeWindowEndTime": "11:57:17.9830000",
  "upgradeAutomatically": true,
  "upgradeAvailable": true,
  "internalNetworkProbeUrl": "https://example.com/internalNetworkProbeUrl/",
  "enableCertificatePinning": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




