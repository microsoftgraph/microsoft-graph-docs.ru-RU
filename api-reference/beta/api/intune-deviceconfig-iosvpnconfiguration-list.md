---
title: Список iosVpnConfigurations
description: Свойства списка и связей объектов iosVpnConfiguration.
author: tfitzmac
ms.openlocfilehash: eeebea3787c5a37baa16a29c0f00a973903bffc0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362848"
---
# <a name="list-iosvpnconfigurations"></a><span data-ttu-id="5996d-103">Список iosVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="5996d-103">List iosVpnConfigurations</span></span>

> <span data-ttu-id="5996d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5996d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5996d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5996d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5996d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5996d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5996d-107">Свойства списка и связей объектов [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5996d-107">List properties and relationships of the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5996d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5996d-108">Prerequisites</span></span>
<span data-ttu-id="5996d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5996d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5996d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5996d-111">Permission type</span></span>|<span data-ttu-id="5996d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5996d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5996d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5996d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5996d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5996d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5996d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5996d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5996d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5996d-116">Not supported.</span></span>|
|<span data-ttu-id="5996d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5996d-117">Application</span></span>|<span data-ttu-id="5996d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5996d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5996d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5996d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5996d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5996d-120">Request headers</span></span>
|<span data-ttu-id="5996d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5996d-121">Header</span></span>|<span data-ttu-id="5996d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5996d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5996d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5996d-123">Authorization</span></span>|<span data-ttu-id="5996d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5996d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5996d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5996d-125">Accept</span></span>|<span data-ttu-id="5996d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5996d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5996d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5996d-127">Request body</span></span>
<span data-ttu-id="5996d-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5996d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5996d-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="5996d-129">Response</span></span>
<span data-ttu-id="5996d-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5996d-130">If successful, this method returns a `200 OK` response code and a collection of [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5996d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5996d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="5996d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5996d-132">Request</span></span>
<span data-ttu-id="5996d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5996d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="5996d-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="5996d-134">Response</span></span>
<span data-ttu-id="5996d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5996d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





