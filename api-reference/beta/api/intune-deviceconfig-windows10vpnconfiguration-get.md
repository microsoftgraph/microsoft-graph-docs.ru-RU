---
title: Получение windows10VpnConfiguration
description: Чтение свойств и связей объекта windows10VpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 16408a8ebe9803c8d6e8f08d90d8370a7db3ab51
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31793366"
---
# <a name="get-windows10vpnconfiguration"></a><span data-ttu-id="9d8e8-103">Получение windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="9d8e8-103">Get windows10VpnConfiguration</span></span>

> <span data-ttu-id="9d8e8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d8e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d8e8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d8e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d8e8-106">Чтение свойств и связей объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9d8e8-106">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d8e8-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9d8e8-107">Prerequisites</span></span>
<span data-ttu-id="9d8e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d8e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d8e8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d8e8-110">Permission type</span></span>|<span data-ttu-id="9d8e8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d8e8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d8e8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d8e8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9d8e8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d8e8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9d8e8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d8e8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d8e8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d8e8-115">Not supported.</span></span>|
|<span data-ttu-id="9d8e8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d8e8-116">Application</span></span>|<span data-ttu-id="9d8e8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d8e8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d8e8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d8e8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9d8e8-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9d8e8-119">Optional query parameters</span></span>
<span data-ttu-id="9d8e8-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9d8e8-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d8e8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d8e8-121">Request headers</span></span>
|<span data-ttu-id="9d8e8-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9d8e8-122">Header</span></span>|<span data-ttu-id="9d8e8-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9d8e8-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d8e8-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d8e8-124">Authorization</span></span>|<span data-ttu-id="9d8e8-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d8e8-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d8e8-126">Accept</span><span class="sxs-lookup"><span data-stu-id="9d8e8-126">Accept</span></span>|<span data-ttu-id="9d8e8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9d8e8-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d8e8-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d8e8-128">Request body</span></span>
<span data-ttu-id="9d8e8-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9d8e8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d8e8-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d8e8-130">Response</span></span>
<span data-ttu-id="9d8e8-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9d8e8-131">If successful, this method returns a `200 OK` response code and [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d8e8-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9d8e8-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d8e8-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d8e8-133">Request</span></span>
<span data-ttu-id="9d8e8-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d8e8-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="9d8e8-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d8e8-135">Response</span></span>
<span data-ttu-id="9d8e8-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d8e8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3814

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
    "id": "c23c9727-9727-c23c-2797-3cc227973cc2",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
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
    ]
  }
}
```





