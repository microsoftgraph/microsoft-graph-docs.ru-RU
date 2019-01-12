---
title: Перечисление объектов iosLobApp
description: Список свойств и связей объектов iosLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f9969da49316443fa1c4ca5a6902368482189362
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982094"
---
# <a name="list-ioslobapps"></a><span data-ttu-id="201e7-103">Перечисление объектов iosLobApp</span><span class="sxs-lookup"><span data-stu-id="201e7-103">List iosLobApps</span></span>

> <span data-ttu-id="201e7-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="201e7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="201e7-105">Список свойств и связей объектов [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="201e7-105">List properties and relationships of the [iosLobApp](../resources/intune-apps-ioslobapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="201e7-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="201e7-106">Prerequisites</span></span>
<span data-ttu-id="201e7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="201e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="201e7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="201e7-109">Permission type</span></span>|<span data-ttu-id="201e7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="201e7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="201e7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="201e7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="201e7-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="201e7-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="201e7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="201e7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="201e7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="201e7-114">Not supported.</span></span>|
|<span data-ttu-id="201e7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="201e7-115">Application</span></span>|<span data-ttu-id="201e7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="201e7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="201e7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="201e7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="201e7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="201e7-118">Request headers</span></span>
|<span data-ttu-id="201e7-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="201e7-119">Header</span></span>|<span data-ttu-id="201e7-120">Значение</span><span class="sxs-lookup"><span data-stu-id="201e7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="201e7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="201e7-121">Authorization</span></span>|<span data-ttu-id="201e7-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="201e7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="201e7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="201e7-123">Accept</span></span>|<span data-ttu-id="201e7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="201e7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="201e7-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="201e7-125">Request body</span></span>
<span data-ttu-id="201e7-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="201e7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="201e7-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="201e7-127">Response</span></span>
<span data-ttu-id="201e7-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosLobApp](../resources/intune-apps-ioslobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="201e7-128">If successful, this method returns a `200 OK` response code and a collection of [iosLobApp](../resources/intune-apps-ioslobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="201e7-129">Пример</span><span class="sxs-lookup"><span data-stu-id="201e7-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="201e7-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="201e7-130">Request</span></span>
<span data-ttu-id="201e7-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="201e7-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="201e7-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="201e7-132">Response</span></span>
<span data-ttu-id="201e7-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="201e7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1570

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosLobApp",
      "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "largeIcon": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "isFeatured": true,
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "informationUrl": "https://example.com/informationUrl/",
      "owner": "Owner value",
      "developer": "Developer value",
      "notes": "Notes value",
      "publishingState": "processing",
      "committedContentVersion": "Committed Content Version value",
      "fileName": "File Name value",
      "size": 4,
      "bundleId": "Bundle Id value",
      "applicableDeviceType": {
        "@odata.type": "microsoft.graph.iosDeviceType",
        "iPad": true,
        "iPhoneAndIPod": true
      },
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
        "v8_0": true,
        "v9_0": true,
        "v10_0": true,
        "v11_0": true,
        "v12_0": true
      },
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "versionNumber": "Version Number value",
      "buildNumber": "Build Number value"
    }
  ]
}
```



