---
title: Список macOSWiFiConfigurations
description: Свойства списка и связей объектов macOSWiFiConfiguration.
ms.openlocfilehash: ea3464a3b6fc3f71d948bb27d0cf48f3dd71cb20
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082252"
---
# <a name="list-macoswificonfigurations"></a><span data-ttu-id="ffd5b-103">Список macOSWiFiConfigurations</span><span class="sxs-lookup"><span data-stu-id="ffd5b-103">List macOSWiFiConfigurations</span></span>

> <span data-ttu-id="ffd5b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ffd5b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ffd5b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ffd5b-107">Свойства списка и связей объектов [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ffd5b-107">List properties and relationships of the [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ffd5b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ffd5b-108">Prerequisites</span></span>
<span data-ttu-id="ffd5b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffd5b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffd5b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffd5b-111">Permission type</span></span>|<span data-ttu-id="ffd5b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffd5b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffd5b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffd5b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ffd5b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ffd5b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ffd5b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffd5b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffd5b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-116">Not supported.</span></span>|
|<span data-ttu-id="ffd5b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ffd5b-117">Application</span></span>|<span data-ttu-id="ffd5b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffd5b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffd5b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ffd5b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ffd5b-120">Request headers</span></span>
|<span data-ttu-id="ffd5b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ffd5b-121">Header</span></span>|<span data-ttu-id="ffd5b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ffd5b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffd5b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffd5b-123">Authorization</span></span>|<span data-ttu-id="ffd5b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ffd5b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffd5b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ffd5b-125">Accept</span></span>|<span data-ttu-id="ffd5b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ffd5b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffd5b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ffd5b-127">Request body</span></span>
<span data-ttu-id="ffd5b-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffd5b-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ffd5b-129">Response</span></span>
<span data-ttu-id="ffd5b-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-130">If successful, this method returns a `200 OK` response code and a collection of [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffd5b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ffd5b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ffd5b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffd5b-132">Request</span></span>
<span data-ttu-id="ffd5b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="ffd5b-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ffd5b-134">Response</span></span>
<span data-ttu-id="ffd5b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ffd5b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 966

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
      "id": "471203fb-03fb-4712-fb03-1247fb031247",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "networkName": "Network Name value",
      "ssid": "Ssid value",
      "connectAutomatically": true,
      "connectWhenNetworkNameIsHidden": true,
      "wiFiSecurityType": "wpaPersonal",
      "proxySettings": "manual",
      "proxyManualAddress": "Proxy Manual Address value",
      "proxyManualPort": 15,
      "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
      "preSharedKey": "Pre Shared Key value"
    }
  ]
}
```





