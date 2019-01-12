---
title: Список windowsPhone81StoreApps
description: Свойства списка и связей объектов windowsPhone81StoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 499f045159fe0364d0bef6843307df8db8cf20be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920165"
---
# <a name="list-windowsphone81storeapps"></a><span data-ttu-id="f849a-103">Список windowsPhone81StoreApps</span><span class="sxs-lookup"><span data-stu-id="f849a-103">List windowsPhone81StoreApps</span></span>

> <span data-ttu-id="f849a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f849a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f849a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f849a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f849a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f849a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f849a-107">Свойства списка и связей объектов [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="f849a-107">List properties and relationships of the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f849a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f849a-108">Prerequisites</span></span>
<span data-ttu-id="f849a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f849a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f849a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f849a-111">Permission type</span></span>|<span data-ttu-id="f849a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f849a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f849a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f849a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f849a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f849a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f849a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f849a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f849a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f849a-116">Not supported.</span></span>|
|<span data-ttu-id="f849a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f849a-117">Application</span></span>|<span data-ttu-id="f849a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f849a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f849a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f849a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f849a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f849a-120">Request headers</span></span>
|<span data-ttu-id="f849a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f849a-121">Header</span></span>|<span data-ttu-id="f849a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f849a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f849a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f849a-123">Authorization</span></span>|<span data-ttu-id="f849a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f849a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f849a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f849a-125">Accept</span></span>|<span data-ttu-id="f849a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f849a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f849a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f849a-127">Request body</span></span>
<span data-ttu-id="f849a-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f849a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f849a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f849a-129">Response</span></span>
<span data-ttu-id="f849a-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f849a-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f849a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f849a-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f849a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f849a-132">Request</span></span>
<span data-ttu-id="f849a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f849a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="f849a-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="f849a-134">Response</span></span>
<span data-ttu-id="f849a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f849a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 952

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81StoreApp",
      "id": "f68ce6a1-e6a1-f68c-a1e6-8cf6a1e68cf6",
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





