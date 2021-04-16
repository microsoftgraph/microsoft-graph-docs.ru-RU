---
title: Список iosVpnConfigurations
description: Список свойств и связей объектов iosVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0b52e4c9859acaadfbeaf9b56eeac8011ed2103d
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868213"
---
# <a name="list-iosvpnconfigurations"></a><span data-ttu-id="3508d-103">Список iosVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="3508d-103">List iosVpnConfigurations</span></span>

<span data-ttu-id="3508d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3508d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3508d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3508d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3508d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3508d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3508d-107">Список свойств и связей объектов [iosVpnConfiguration.](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3508d-107">List properties and relationships of the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3508d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3508d-108">Prerequisites</span></span>
<span data-ttu-id="3508d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3508d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3508d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3508d-111">Permission type</span></span>|<span data-ttu-id="3508d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3508d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3508d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3508d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3508d-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3508d-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3508d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3508d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3508d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3508d-116">Not supported.</span></span>|
|<span data-ttu-id="3508d-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="3508d-117">Application</span></span>|<span data-ttu-id="3508d-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3508d-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3508d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3508d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3508d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3508d-120">Request headers</span></span>
|<span data-ttu-id="3508d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3508d-121">Header</span></span>|<span data-ttu-id="3508d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3508d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3508d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3508d-123">Authorization</span></span>|<span data-ttu-id="3508d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3508d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3508d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3508d-125">Accept</span></span>|<span data-ttu-id="3508d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3508d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3508d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3508d-127">Request body</span></span>
<span data-ttu-id="3508d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3508d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3508d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3508d-129">Response</span></span>
<span data-ttu-id="3508d-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3508d-130">If successful, this method returns a `200 OK` response code and a collection of [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3508d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3508d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3508d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3508d-132">Request</span></span>
<span data-ttu-id="3508d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3508d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="3508d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3508d-134">Response</span></span>
<span data-ttu-id="3508d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3508d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4033

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
      "disconnectOnIdle": true,
      "disconnectOnIdleTimerInSeconds": 14,
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




