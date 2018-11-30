---
title: Список windowsStoreApps
description: Свойства списка и связей объектов windowsStoreApp.
ms.openlocfilehash: 160dcd619cde68197438693c108e06834755a102
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078223"
---
# <a name="list-windowsstoreapps"></a><span data-ttu-id="e72e0-103">Список windowsStoreApps</span><span class="sxs-lookup"><span data-stu-id="e72e0-103">List windowsStoreApps</span></span>

> <span data-ttu-id="e72e0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e72e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e72e0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e72e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e72e0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e72e0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e72e0-107">Свойства списка и связей объектов [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="e72e0-107">List properties and relationships of the [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e72e0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e72e0-108">Prerequisites</span></span>
<span data-ttu-id="e72e0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e72e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e72e0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e72e0-111">Permission type</span></span>|<span data-ttu-id="e72e0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e72e0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e72e0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e72e0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e72e0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e72e0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e72e0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e72e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e72e0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e72e0-116">Not supported.</span></span>|
|<span data-ttu-id="e72e0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e72e0-117">Application</span></span>|<span data-ttu-id="e72e0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e72e0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e72e0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e72e0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e72e0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e72e0-120">Request headers</span></span>
|<span data-ttu-id="e72e0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e72e0-121">Header</span></span>|<span data-ttu-id="e72e0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e72e0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e72e0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e72e0-123">Authorization</span></span>|<span data-ttu-id="e72e0-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e72e0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e72e0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e72e0-125">Accept</span></span>|<span data-ttu-id="e72e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e72e0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e72e0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e72e0-127">Request body</span></span>
<span data-ttu-id="e72e0-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e72e0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e72e0-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="e72e0-129">Response</span></span>
<span data-ttu-id="e72e0-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e72e0-130">If successful, this method returns a `200 OK` response code and a collection of [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e72e0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e72e0-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e72e0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e72e0-132">Request</span></span>
<span data-ttu-id="e72e0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e72e0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="e72e0-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="e72e0-134">Response</span></span>
<span data-ttu-id="e72e0-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e72e0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 945

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsStoreApp",
      "id": "fd4a5f8a-5f8a-fd4a-8a5f-4afd8a5f4afd",
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
      "appStoreUrl": "https://example.com/appStoreUrl/"
    }
  ]
}
```





