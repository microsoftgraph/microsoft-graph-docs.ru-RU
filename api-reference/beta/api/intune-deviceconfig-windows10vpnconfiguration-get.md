---
title: Получить windows10VpnConfiguration
description: Чтение свойств и связей объекта Windows10VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 22008d8e569634fb0652b5b3a970b00adbfd1dbd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127335"
---
# <a name="get-windows10vpnconfiguration"></a><span data-ttu-id="f6678-103">Получить windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f6678-103">Get windows10VpnConfiguration</span></span>

<span data-ttu-id="f6678-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6678-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6678-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6678-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6678-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f6678-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6678-107">Чтение свойств и связей [объекта Windows10VpnConfiguration.](../resources/intune-deviceconfig-windows10vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f6678-107">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6678-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f6678-108">Prerequisites</span></span>
<span data-ttu-id="f6678-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6678-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6678-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6678-111">Permission type</span></span>|<span data-ttu-id="f6678-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6678-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6678-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6678-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6678-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6678-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f6678-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6678-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6678-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6678-116">Not supported.</span></span>|
|<span data-ttu-id="f6678-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f6678-117">Application</span></span>|<span data-ttu-id="f6678-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6678-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6678-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6678-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6678-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f6678-120">Optional query parameters</span></span>
<span data-ttu-id="f6678-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f6678-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6678-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6678-122">Request headers</span></span>
|<span data-ttu-id="f6678-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6678-123">Header</span></span>|<span data-ttu-id="f6678-124">Значение</span><span class="sxs-lookup"><span data-stu-id="f6678-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6678-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6678-125">Authorization</span></span>|<span data-ttu-id="f6678-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6678-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6678-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f6678-127">Accept</span></span>|<span data-ttu-id="f6678-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f6678-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6678-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6678-129">Request body</span></span>
<span data-ttu-id="f6678-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6678-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6678-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6678-131">Response</span></span>
<span data-ttu-id="f6678-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект Windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f6678-132">If successful, this method returns a `200 OK` response code and [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6678-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f6678-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6678-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6678-134">Request</span></span>
<span data-ttu-id="f6678-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6678-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f6678-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6678-136">Response</span></span>
<span data-ttu-id="f6678-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6678-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4950

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
    "id": "c23c9727-9727-c23c-2797-3cc227973cc2",
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
    "servers": [
      {
        "@odata.type": "microsoft.graph.vpnServer",
        "description": "Description value",
        "address": "Address value",
        "isDefaultServer": true
      }
    ],
    "customXml": "Y3VzdG9tWG1s",
    "profileTarget": "device",
    "connectionType": "f5EdgeClient",
    "enableSplitTunneling": true,
    "enableAlwaysOn": true,
    "enableDeviceTunnel": true,
    "enableDnsRegistration": true,
    "dnsSuffixes": [
      "Dns Suffixes value"
    ],
    "authenticationMethod": "usernameAndPassword",
    "rememberUserCredentials": true,
    "enableConditionalAccess": true,
    "enableSingleSignOnWithAlternateCertificate": true,
    "singleSignOnEku": {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    },
    "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
    "eapXml": "ZWFwWG1s",
    "proxyServer": {
      "@odata.type": "microsoft.graph.windows10VpnProxyServer",
      "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
      "address": "Address value",
      "port": 4,
      "bypassProxyServerForLocalAddress": true
    },
    "associatedApps": [
      {
        "@odata.type": "microsoft.graph.windows10AssociatedApps",
        "appType": "universal",
        "identifier": "Identifier value"
      }
    ],
    "onlyAssociatedAppsCanUseConnection": true,
    "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
    "trafficRules": [
      {
        "@odata.type": "microsoft.graph.vpnTrafficRule",
        "name": "Name value",
        "protocols": 9,
        "localPortRanges": [
          {
            "@odata.type": "microsoft.graph.numberRange",
            "lowerNumber": 11,
            "upperNumber": 11
          }
        ],
        "remotePortRanges": [
          {
            "@odata.type": "microsoft.graph.numberRange",
            "lowerNumber": 11,
            "upperNumber": 11
          }
        ],
        "localAddressRanges": [
          {
            "@odata.type": "microsoft.graph.iPv4Range",
            "lowerAddress": "Lower Address value",
            "upperAddress": "Upper Address value"
          }
        ],
        "remoteAddressRanges": [
          {
            "@odata.type": "microsoft.graph.iPv4Range",
            "lowerAddress": "Lower Address value",
            "upperAddress": "Upper Address value"
          }
        ],
        "appId": "App Id value",
        "appType": "desktop",
        "routingPolicyType": "splitTunnel",
        "claims": "Claims value"
      }
    ],
    "routes": [
      {
        "@odata.type": "microsoft.graph.vpnRoute",
        "destinationPrefix": "Destination Prefix value",
        "prefixSize": 10
      }
    ],
    "dnsRules": [
      {
        "@odata.type": "microsoft.graph.vpnDnsRule",
        "name": "Name value",
        "servers": [
          "Servers value"
        ],
        "proxyServerUri": "Proxy Server Uri value",
        "autoTrigger": true,
        "persistent": true
      }
    ],
    "trustedNetworkDomains": [
      "Trusted Network Domains value"
    ],
    "cryptographySuite": {
      "@odata.type": "microsoft.graph.cryptographySuite",
      "encryptionMethod": "des",
      "integrityCheckMethod": "sha1_96",
      "dhGroup": "group2",
      "cipherTransformConstants": "des",
      "authenticationTransformConstants": "sha1_96",
      "pfsGroup": "pfs2"
    }
  }
}
```




