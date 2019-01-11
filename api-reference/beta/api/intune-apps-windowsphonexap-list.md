---
title: Список windowsPhoneXAPs
description: Свойства списка и связей объектов windowsPhoneXAP.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f2e683ea10bbea78f5364b21168b8e99cee9a4ab
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875112"
---
# <a name="list-windowsphonexaps"></a><span data-ttu-id="a1bac-103">Список windowsPhoneXAPs</span><span class="sxs-lookup"><span data-stu-id="a1bac-103">List windowsPhoneXAPs</span></span>

> <span data-ttu-id="a1bac-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a1bac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1bac-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1bac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a1bac-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a1bac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1bac-107">Свойства списка и связей объектов [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) .</span><span class="sxs-lookup"><span data-stu-id="a1bac-107">List properties and relationships of the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a1bac-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a1bac-108">Prerequisites</span></span>
<span data-ttu-id="a1bac-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1bac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1bac-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1bac-111">Permission type</span></span>|<span data-ttu-id="a1bac-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1bac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1bac-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1bac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1bac-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1bac-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a1bac-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1bac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1bac-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1bac-116">Not supported.</span></span>|
|<span data-ttu-id="a1bac-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1bac-117">Application</span></span>|<span data-ttu-id="a1bac-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1bac-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1bac-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1bac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a1bac-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1bac-120">Request headers</span></span>
|<span data-ttu-id="a1bac-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a1bac-121">Header</span></span>|<span data-ttu-id="a1bac-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a1bac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1bac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1bac-123">Authorization</span></span>|<span data-ttu-id="a1bac-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a1bac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1bac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a1bac-125">Accept</span></span>|<span data-ttu-id="a1bac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a1bac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1bac-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a1bac-127">Request body</span></span>
<span data-ttu-id="a1bac-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a1bac-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1bac-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="a1bac-129">Response</span></span>
<span data-ttu-id="a1bac-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a1bac-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1bac-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a1bac-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a1bac-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1bac-132">Request</span></span>
<span data-ttu-id="a1bac-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1bac-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="a1bac-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a1bac-134">Response</span></span>
<span data-ttu-id="a1bac-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a1bac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1424

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhoneXAP",
      "id": "301ddc77-dc77-301d-77dc-1d3077dc1d30",
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
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true
      },
      "productIdentifier": "Product Identifier value",
      "identityVersion": "Identity Version value"
    }
  ]
}
```





