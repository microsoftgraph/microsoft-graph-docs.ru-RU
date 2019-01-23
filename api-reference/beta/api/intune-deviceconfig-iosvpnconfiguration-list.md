---
title: Список iosVpnConfigurations
description: Свойства списка и связей объектов iosVpnConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 54a3273006d18a178ae4a4b4d83485d1c4c5a34c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392950"
---
# <a name="list-iosvpnconfigurations"></a><span data-ttu-id="be065-103">Список iosVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="be065-103">List iosVpnConfigurations</span></span>

> <span data-ttu-id="be065-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="be065-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="be065-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be065-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="be065-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be065-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be065-107">Свойства списка и связей объектов [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="be065-107">List properties and relationships of the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be065-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="be065-108">Prerequisites</span></span>
<span data-ttu-id="be065-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="be065-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="be065-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be065-111">Permission type</span></span>|<span data-ttu-id="be065-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="be065-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be065-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be065-113">Delegated (work or school account)</span></span>|<span data-ttu-id="be065-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="be065-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="be065-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be065-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be065-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be065-116">Not supported.</span></span>|
|<span data-ttu-id="be065-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be065-117">Application</span></span>|<span data-ttu-id="be065-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be065-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be065-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be065-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="be065-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be065-120">Request headers</span></span>
|<span data-ttu-id="be065-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be065-121">Header</span></span>|<span data-ttu-id="be065-122">Значение</span><span class="sxs-lookup"><span data-stu-id="be065-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be065-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="be065-123">Authorization</span></span>|<span data-ttu-id="be065-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="be065-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be065-125">Accept</span><span class="sxs-lookup"><span data-stu-id="be065-125">Accept</span></span>|<span data-ttu-id="be065-126">application/json</span><span class="sxs-lookup"><span data-stu-id="be065-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be065-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be065-127">Request body</span></span>
<span data-ttu-id="be065-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="be065-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be065-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="be065-129">Response</span></span>
<span data-ttu-id="be065-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="be065-130">If successful, this method returns a `200 OK` response code and a collection of [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be065-131">Пример</span><span class="sxs-lookup"><span data-stu-id="be065-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="be065-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="be065-132">Request</span></span>
<span data-ttu-id="be065-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be065-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="be065-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="be065-134">Response</span></span>
<span data-ttu-id="be065-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="be065-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2547

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
      ]
    }
  ]
}
```




