---
title: Получение iosikEv2VpnConfiguration
description: Чтение свойств и связей объекта iosikEv2VpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 832213335bd06d1bd2c739e011055c02d7163f58
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41635911"
---
# <a name="get-iosikev2vpnconfiguration"></a><span data-ttu-id="1348b-103">Получение iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="1348b-103">Get iosikEv2VpnConfiguration</span></span>

> <span data-ttu-id="1348b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1348b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1348b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1348b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1348b-106">Чтение свойств и связей объекта [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1348b-106">Read properties and relationships of the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1348b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1348b-107">Prerequisites</span></span>
<span data-ttu-id="1348b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1348b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1348b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1348b-110">Permission type</span></span>|<span data-ttu-id="1348b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1348b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1348b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1348b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1348b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1348b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1348b-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1348b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1348b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1348b-115">Not supported.</span></span>|
|<span data-ttu-id="1348b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1348b-116">Application</span></span>|<span data-ttu-id="1348b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1348b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1348b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1348b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1348b-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1348b-119">Optional query parameters</span></span>
<span data-ttu-id="1348b-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1348b-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1348b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1348b-121">Request headers</span></span>
|<span data-ttu-id="1348b-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1348b-122">Header</span></span>|<span data-ttu-id="1348b-123">Значение</span><span class="sxs-lookup"><span data-stu-id="1348b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1348b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1348b-124">Authorization</span></span>|<span data-ttu-id="1348b-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1348b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1348b-126">Accept</span><span class="sxs-lookup"><span data-stu-id="1348b-126">Accept</span></span>|<span data-ttu-id="1348b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1348b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1348b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1348b-128">Request body</span></span>
<span data-ttu-id="1348b-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1348b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1348b-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="1348b-130">Response</span></span>
<span data-ttu-id="1348b-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1348b-131">If successful, this method returns a `200 OK` response code and [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1348b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="1348b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1348b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1348b-133">Request</span></span>
<span data-ttu-id="1348b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1348b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="1348b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1348b-135">Response</span></span>
<span data-ttu-id="1348b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1348b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5469

{
  "value": {
    "@odata.type": "#microsoft.graph.iosikEv2VpnConfiguration",
    "id": "b87b0327-0327-b87b-2703-7bb827037bb8",
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
    "proxyServer": {
      "@odata.type": "microsoft.graph.vpnProxyServer",
      "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
      "address": "Address value",
      "port": 4
    },
    "optInToDeviceIdSharing": true,
    "providerType": "appProxy",
    "userDomain": "User Domain value",
    "strictEnforcement": true,
    "cloudName": "Cloud Name value",
    "excludeList": [
      "Exclude List value"
    ],
    "childSecurityAssociationParameters": {
      "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
      "securityEncryptionAlgorithm": "des",
      "securityIntegrityAlgorithm": "sha1_96",
      "securityDiffieHellmanGroup": 10,
      "lifetimeInMinutes": 1
    },
    "clientAuthenticationType": "deviceAuthentication",
    "deadPeerDetectionRate": "none",
    "disableMobilityAndMultihoming": true,
    "disableRedirect": true,
    "enableCertificateRevocationCheck": true,
    "enableEAP": true,
    "enablePerfectForwardSecrecy": true,
    "enableUseInternalSubnetAttributes": true,
    "localIdentifier": "empty",
    "remoteIdentifier": "Remote Identifier value",
    "securityAssociationParameters": {
      "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
      "securityEncryptionAlgorithm": "des",
      "securityIntegrityAlgorithm": "sha1_96",
      "securityDiffieHellmanGroup": 10,
      "lifetimeInMinutes": 1
    },
    "serverCertificateCommonName": "Server Certificate Common Name value",
    "serverCertificateIssuerCommonName": "Server Certificate Issuer Common Name value",
    "serverCertificateType": "ecdsa256",
    "sharedSecret": "Shared Secret value",
    "tlsMaximumVersion": "Tls Maximum Version value",
    "tlsMinimumVersion": "Tls Minimum Version value",
    "allowDefaultSecurityAssociationParameters": true,
    "allowDefaultChildSecurityAssociationParameters": true,
    "alwaysOnConfiguration": {
      "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration",
      "tunnelConfiguration": "cellular",
      "userToggleEnabled": true,
      "voicemailExceptionAction": "allowTrafficOutside",
      "airPrintExceptionAction": "allowTrafficOutside",
      "cellularExceptionAction": "allowTrafficOutside",
      "allowAllCaptiveNetworkPlugins": true,
      "allowedCaptiveNetworkPlugins": {
        "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins",
        "allowedBundleIdentifiers": [
          "Allowed Bundle Identifiers value"
        ]
      },
      "allowCaptiveWebSheet": true,
      "natKeepAliveIntervalInSeconds": 13,
      "natKeepAliveOffloadEnable": true
    },
    "enableAlwaysOnConfiguration": true
  }
}
```





