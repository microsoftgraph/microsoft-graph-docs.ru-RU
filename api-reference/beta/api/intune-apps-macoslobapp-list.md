---
title: Список macOSLobApps
description: Свойства списка и связей объектов macOSLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0425a1444deac68baf69d698b622133dec5d0205
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969361"
---
# <a name="list-macoslobapps"></a><span data-ttu-id="d665f-103">Список macOSLobApps</span><span class="sxs-lookup"><span data-stu-id="d665f-103">List macOSLobApps</span></span>

> <span data-ttu-id="d665f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d665f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d665f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d665f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d665f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d665f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d665f-107">Свойства списка и связей объектов [macOSLobApp](../resources/intune-apps-macoslobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="d665f-107">List properties and relationships of the [macOSLobApp](../resources/intune-apps-macoslobapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d665f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d665f-108">Prerequisites</span></span>
<span data-ttu-id="d665f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d665f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d665f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d665f-111">Permission type</span></span>|<span data-ttu-id="d665f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d665f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d665f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d665f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d665f-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d665f-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d665f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d665f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d665f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d665f-116">Not supported.</span></span>|
|<span data-ttu-id="d665f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d665f-117">Application</span></span>|<span data-ttu-id="d665f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d665f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d665f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d665f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d665f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d665f-120">Request headers</span></span>
|<span data-ttu-id="d665f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d665f-121">Header</span></span>|<span data-ttu-id="d665f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d665f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d665f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d665f-123">Authorization</span></span>|<span data-ttu-id="d665f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d665f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d665f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d665f-125">Accept</span></span>|<span data-ttu-id="d665f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d665f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d665f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d665f-127">Request body</span></span>
<span data-ttu-id="d665f-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d665f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d665f-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="d665f-129">Response</span></span>
<span data-ttu-id="d665f-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [macOSLobApp](../resources/intune-apps-macoslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d665f-130">If successful, this method returns a `200 OK` response code and a collection of [macOSLobApp](../resources/intune-apps-macoslobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d665f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d665f-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d665f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d665f-132">Request</span></span>
<span data-ttu-id="d665f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d665f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="d665f-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="d665f-134">Response</span></span>
<span data-ttu-id="d665f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d665f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1867

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSLobApp",
      "id": "7be9250a-250a-7be9-0a25-e97b0a25e97b",
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
      "uploadState": 11,
      "publishingState": "processing",
      "committedContentVersion": "Committed Content Version value",
      "fileName": "File Name value",
      "size": 4,
      "bundleId": "Bundle Id value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
        "v10_7": true,
        "v10_8": true,
        "v10_9": true,
        "v10_10": true,
        "v10_11": true,
        "v10_12": true,
        "v10_13": true
      },
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value",
      "childApps": [
        {
          "@odata.type": "microsoft.graph.macOSLobChildApp",
          "bundleId": "Bundle Id value",
          "buildNumber": "Build Number value",
          "versionNumber": "Version Number value"
        }
      ],
      "identityVersion": "Identity Version value",
      "md5HashChunkSize": 0,
      "md5Hash": [
        "Md5Hash value"
      ],
      "ignoreVersionDetection": true
    }
  ]
}
```





