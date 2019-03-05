---
title: Список Макосвпнконфигуратионс
description: Список свойств и связей объектов Макосвпнконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a2cb4db321f323e80714280c2c4c6c3b5df7f59
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144893"
---
# <a name="list-macosvpnconfigurations"></a><span data-ttu-id="ee99a-103">Список Макосвпнконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="ee99a-103">List macOSVpnConfigurations</span></span>

> <span data-ttu-id="ee99a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee99a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee99a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee99a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee99a-106">Список свойств и связей объектов [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ee99a-106">List properties and relationships of the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee99a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ee99a-107">Prerequisites</span></span>
<span data-ttu-id="ee99a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ee99a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ee99a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee99a-110">Permission type</span></span>|<span data-ttu-id="ee99a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee99a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee99a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee99a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ee99a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee99a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ee99a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee99a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee99a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee99a-115">Not supported.</span></span>|
|<span data-ttu-id="ee99a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee99a-116">Application</span></span>|<span data-ttu-id="ee99a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee99a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee99a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee99a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ee99a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee99a-119">Request headers</span></span>
|<span data-ttu-id="ee99a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee99a-120">Header</span></span>|<span data-ttu-id="ee99a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ee99a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee99a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee99a-122">Authorization</span></span>|<span data-ttu-id="ee99a-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ee99a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee99a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ee99a-124">Accept</span></span>|<span data-ttu-id="ee99a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ee99a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee99a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee99a-126">Request body</span></span>
<span data-ttu-id="ee99a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ee99a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee99a-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee99a-128">Response</span></span>
<span data-ttu-id="ee99a-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ee99a-129">If successful, this method returns a `200 OK` response code and a collection of [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee99a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ee99a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee99a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee99a-131">Request</span></span>
<span data-ttu-id="ee99a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee99a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="ee99a-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee99a-133">Response</span></span>
<span data-ttu-id="ee99a-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee99a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2334

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
      "optInToDeviceIdSharing": true
    }
  ]
}
```




