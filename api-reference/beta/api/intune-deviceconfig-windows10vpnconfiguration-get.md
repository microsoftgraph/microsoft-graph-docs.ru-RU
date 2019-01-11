---
title: Получение windows10VpnConfiguration
description: Чтение свойства и связи объекта windows10VpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9e8d3dd31801ad7786add430d4dba2edf26335eb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833680"
---
# <a name="get-windows10vpnconfiguration"></a><span data-ttu-id="19698-103">Получение windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="19698-103">Get windows10VpnConfiguration</span></span>

> <span data-ttu-id="19698-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="19698-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19698-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19698-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19698-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="19698-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19698-107">Чтение свойства и связи объекта [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="19698-107">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="19698-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="19698-108">Prerequisites</span></span>
<span data-ttu-id="19698-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19698-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19698-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19698-111">Permission type</span></span>|<span data-ttu-id="19698-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="19698-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19698-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19698-113">Delegated (work or school account)</span></span>|<span data-ttu-id="19698-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="19698-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="19698-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19698-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19698-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19698-116">Not supported.</span></span>|
|<span data-ttu-id="19698-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19698-117">Application</span></span>|<span data-ttu-id="19698-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19698-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19698-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19698-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19698-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="19698-120">Optional query parameters</span></span>
<span data-ttu-id="19698-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="19698-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="19698-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19698-122">Request headers</span></span>
|<span data-ttu-id="19698-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19698-123">Header</span></span>|<span data-ttu-id="19698-124">Значение</span><span class="sxs-lookup"><span data-stu-id="19698-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19698-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="19698-125">Authorization</span></span>|<span data-ttu-id="19698-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="19698-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19698-127">Accept</span><span class="sxs-lookup"><span data-stu-id="19698-127">Accept</span></span>|<span data-ttu-id="19698-128">application/json</span><span class="sxs-lookup"><span data-stu-id="19698-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19698-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="19698-129">Request body</span></span>
<span data-ttu-id="19698-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="19698-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19698-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="19698-131">Response</span></span>
<span data-ttu-id="19698-132">Успешно завершена, этот метод возвращает `200 OK` объект [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="19698-132">If successful, this method returns a `200 OK` response code and [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19698-133">Пример</span><span class="sxs-lookup"><span data-stu-id="19698-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="19698-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="19698-134">Request</span></span>
<span data-ttu-id="19698-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19698-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="19698-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="19698-136">Response</span></span>
<span data-ttu-id="19698-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="19698-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3676

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
        "proxyServerUri": "Proxy Server Uri value"
      }
    ]
  }
}
```





