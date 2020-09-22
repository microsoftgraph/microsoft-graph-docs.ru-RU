---
title: Список Макосвпнконфигуратионс
description: Список свойств и связей объектов Макосвпнконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5ecaf0fb67a1072040b000484f591f04b560840e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017874"
---
# <a name="list-macosvpnconfigurations"></a><span data-ttu-id="22780-103">Список Макосвпнконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="22780-103">List macOSVpnConfigurations</span></span>

<span data-ttu-id="22780-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22780-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22780-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22780-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22780-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="22780-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22780-107">Список свойств и связей объектов [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="22780-107">List properties and relationships of the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22780-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="22780-108">Prerequisites</span></span>
<span data-ttu-id="22780-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22780-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22780-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22780-111">Permission type</span></span>|<span data-ttu-id="22780-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="22780-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22780-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22780-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22780-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="22780-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="22780-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22780-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22780-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22780-116">Not supported.</span></span>|
|<span data-ttu-id="22780-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22780-117">Application</span></span>|<span data-ttu-id="22780-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="22780-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22780-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22780-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="22780-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="22780-120">Request headers</span></span>
|<span data-ttu-id="22780-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22780-121">Header</span></span>|<span data-ttu-id="22780-122">Значение</span><span class="sxs-lookup"><span data-stu-id="22780-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22780-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="22780-123">Authorization</span></span>|<span data-ttu-id="22780-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22780-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22780-125">Accept</span><span class="sxs-lookup"><span data-stu-id="22780-125">Accept</span></span>|<span data-ttu-id="22780-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22780-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22780-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22780-127">Request body</span></span>
<span data-ttu-id="22780-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="22780-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22780-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="22780-129">Response</span></span>
<span data-ttu-id="22780-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="22780-130">If successful, this method returns a `200 OK` response code and a collection of [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22780-131">Пример</span><span class="sxs-lookup"><span data-stu-id="22780-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="22780-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="22780-132">Request</span></span>
<span data-ttu-id="22780-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22780-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="22780-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="22780-134">Response</span></span>
<span data-ttu-id="22780-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22780-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3342

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
      "id": "8ce00178-0178-8ce0-7801-e08c7801e08c",
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
      "optInToDeviceIdSharing": true
    }
  ]
}
```






