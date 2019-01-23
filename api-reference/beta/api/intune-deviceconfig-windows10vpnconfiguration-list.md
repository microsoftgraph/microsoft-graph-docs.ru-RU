---
title: Список windows10VpnConfigurations
description: Свойства списка и связей объектов windows10VpnConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6f3c19a5690aa21433aecc08c730ef4942b6f314
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424303"
---
# <a name="list-windows10vpnconfigurations"></a><span data-ttu-id="bd6de-103">Список windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="bd6de-103">List windows10VpnConfigurations</span></span>

> <span data-ttu-id="bd6de-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bd6de-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bd6de-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd6de-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd6de-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd6de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd6de-107">Свойства списка и связей объектов [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="bd6de-107">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd6de-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="bd6de-108">Prerequisites</span></span>
<span data-ttu-id="bd6de-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bd6de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bd6de-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd6de-111">Permission type</span></span>|<span data-ttu-id="bd6de-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd6de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd6de-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd6de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bd6de-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd6de-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bd6de-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd6de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd6de-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd6de-116">Not supported.</span></span>|
|<span data-ttu-id="bd6de-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd6de-117">Application</span></span>|<span data-ttu-id="bd6de-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd6de-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd6de-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd6de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bd6de-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd6de-120">Request headers</span></span>
|<span data-ttu-id="bd6de-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bd6de-121">Header</span></span>|<span data-ttu-id="bd6de-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bd6de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd6de-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd6de-123">Authorization</span></span>|<span data-ttu-id="bd6de-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bd6de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd6de-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bd6de-125">Accept</span></span>|<span data-ttu-id="bd6de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bd6de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd6de-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd6de-127">Request body</span></span>
<span data-ttu-id="bd6de-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bd6de-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd6de-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd6de-129">Response</span></span>
<span data-ttu-id="bd6de-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bd6de-130">If successful, this method returns a `200 OK` response code and a collection of [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd6de-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bd6de-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd6de-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd6de-132">Request</span></span>
<span data-ttu-id="bd6de-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd6de-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="bd6de-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd6de-134">Response</span></span>
<span data-ttu-id="bd6de-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bd6de-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




