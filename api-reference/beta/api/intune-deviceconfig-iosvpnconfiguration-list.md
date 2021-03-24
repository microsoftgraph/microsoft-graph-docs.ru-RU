---
title: Список iosVpnConfigurations
description: Список свойств и связей объектов iosVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cb5cd620c884a153a10a07e632273db3345a6586
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129862"
---
# <a name="list-iosvpnconfigurations"></a><span data-ttu-id="f5b47-103">Список iosVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="f5b47-103">List iosVpnConfigurations</span></span>

<span data-ttu-id="f5b47-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5b47-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5b47-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5b47-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5b47-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f5b47-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5b47-107">Список свойств и связей объектов [iosVpnConfiguration.](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5b47-107">List properties and relationships of the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5b47-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f5b47-108">Prerequisites</span></span>
<span data-ttu-id="f5b47-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5b47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5b47-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5b47-111">Permission type</span></span>|<span data-ttu-id="f5b47-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5b47-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5b47-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5b47-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f5b47-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5b47-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f5b47-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5b47-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5b47-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5b47-116">Not supported.</span></span>|
|<span data-ttu-id="f5b47-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f5b47-117">Application</span></span>|<span data-ttu-id="f5b47-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5b47-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5b47-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5b47-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f5b47-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f5b47-120">Request headers</span></span>
|<span data-ttu-id="f5b47-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f5b47-121">Header</span></span>|<span data-ttu-id="f5b47-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f5b47-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5b47-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5b47-123">Authorization</span></span>|<span data-ttu-id="f5b47-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5b47-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5b47-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f5b47-125">Accept</span></span>|<span data-ttu-id="f5b47-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f5b47-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5b47-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5b47-127">Request body</span></span>
<span data-ttu-id="f5b47-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f5b47-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5b47-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5b47-129">Response</span></span>
<span data-ttu-id="f5b47-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f5b47-130">If successful, this method returns a `200 OK` response code and a collection of [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5b47-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f5b47-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5b47-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5b47-132">Request</span></span>
<span data-ttu-id="f5b47-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5b47-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="f5b47-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5b47-134">Response</span></span>
<span data-ttu-id="f5b47-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f5b47-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3955

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVpnConfiguration",
      "id": "bd12424c-424c-bd12-4c42-12bd4c4212bd",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "deviceManagementApplicabilityRuleOsEdition": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
        "osEditionTypes": [
          "windows10EnterpriseN"
        ],
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleOsVersion": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
        "minOSVersion": "Min OSVersion value",
        "maxOSVersion": "Max OSVersion value",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleDeviceMode": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
        "deviceMode": "sModeConfiguration",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "connectionName": "Connection Name value",
      "connectionType": "pulseSecure",
      "loginGroupOrDomain": "Login Group Or Domain value",
      "role": "Role value",
      "realm": "Realm value",
      "server": {
        "@odata.type": "microsoft.graph.vpnServer",
        "description": "Description value",
        "address": "Address value",
        "isDefaultServer": true
      },
      "identifier": "Identifier value",
      "customData": [
        {
          "@odata.type": "microsoft.graph.keyValue",
          "key": "Key value",
          "value": "Value value"
        }
      ],
      "customKeyValueData": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "enableSplitTunneling": true,
      "authenticationMethod": "usernameAndPassword",
      "enablePerApp": true,
      "safariDomains": [
        "Safari Domains value"
      ],
      "onDemandRules": [
        {
          "@odata.type": "microsoft.graph.vpnOnDemandRule",
          "ssids": [
            "Ssids value"
          ],
          "dnsSearchDomains": [
            "Dns Search Domains value"
          ],
          "probeUrl": "https://example.com/probeUrl/",
          "action": "evaluateConnection",
          "domainAction": "neverConnect",
          "domains": [
            "Domains value"
          ],
          "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
        }
      ],
      "providerType": "appProxy",
      "associatedDomains": [
        "Associated Domains value"
      ],
      "excludedDomains": [
        "Excluded Domains value"
      ],
      "disableOnDemandUserOverride": true,
      "proxyServer": {
        "@odata.type": "microsoft.graph.vpnProxyServer",
        "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
        "address": "Address value",
        "port": 4
      },
      "optInToDeviceIdSharing": true,
      "userDomain": "User Domain value",
      "strictEnforcement": true,
      "cloudName": "Cloud Name value",
      "excludeList": [
        "Exclude List value"
      ],
      "targetedMobileApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value"
    }
  ]
}
```




