---
title: Список windows10VpnConfigurations
description: Список свойств и связей объектов windows10VpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69d588ec5fa433492de0fcdcff1d55ad9fe1bed9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31778896"
---
# <a name="list-windows10vpnconfigurations"></a><span data-ttu-id="75a58-103">Список windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="75a58-103">List windows10VpnConfigurations</span></span>

> <span data-ttu-id="75a58-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75a58-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75a58-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75a58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75a58-106">Список свойств и связей объектов [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="75a58-106">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75a58-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="75a58-107">Prerequisites</span></span>
<span data-ttu-id="75a58-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75a58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75a58-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75a58-110">Permission type</span></span>|<span data-ttu-id="75a58-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="75a58-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75a58-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75a58-112">Delegated (work or school account)</span></span>|<span data-ttu-id="75a58-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="75a58-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="75a58-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75a58-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75a58-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75a58-115">Not supported.</span></span>|
|<span data-ttu-id="75a58-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75a58-116">Application</span></span>|<span data-ttu-id="75a58-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75a58-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75a58-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75a58-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="75a58-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75a58-119">Request headers</span></span>
|<span data-ttu-id="75a58-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75a58-120">Header</span></span>|<span data-ttu-id="75a58-121">Значение</span><span class="sxs-lookup"><span data-stu-id="75a58-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75a58-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75a58-122">Authorization</span></span>|<span data-ttu-id="75a58-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75a58-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75a58-124">Accept</span><span class="sxs-lookup"><span data-stu-id="75a58-124">Accept</span></span>|<span data-ttu-id="75a58-125">application/json</span><span class="sxs-lookup"><span data-stu-id="75a58-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75a58-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75a58-126">Request body</span></span>
<span data-ttu-id="75a58-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75a58-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75a58-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="75a58-128">Response</span></span>
<span data-ttu-id="75a58-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="75a58-129">If successful, this method returns a `200 OK` response code and a collection of [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75a58-130">Пример</span><span class="sxs-lookup"><span data-stu-id="75a58-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="75a58-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="75a58-131">Request</span></span>
<span data-ttu-id="75a58-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75a58-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="75a58-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="75a58-133">Response</span></span>
<span data-ttu-id="75a58-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75a58-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4064

{
  "value": [
    {
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
  ]
}
```





