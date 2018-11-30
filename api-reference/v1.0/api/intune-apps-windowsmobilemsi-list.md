---
title: Перечисление объектов windowsMobileMSI
description: Список свойств и связей объектов windowsMobileMSI.
ms.openlocfilehash: d384b96c904f9f643007118d601ea7dbb24960bf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027661"
---
# <a name="list-windowsmobilemsis"></a><span data-ttu-id="535a1-103">Перечисление объектов windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="535a1-103">List windowsMobileMSIs</span></span>

> <span data-ttu-id="535a1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="535a1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="535a1-105">Список свойств и связей объектов [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="535a1-105">List properties and relationships of the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="535a1-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="535a1-106">Prerequisites</span></span>
<span data-ttu-id="535a1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="535a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="535a1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="535a1-109">Permission type</span></span>|<span data-ttu-id="535a1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="535a1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="535a1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="535a1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="535a1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="535a1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="535a1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="535a1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="535a1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="535a1-114">Not supported.</span></span>|
|<span data-ttu-id="535a1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="535a1-115">Application</span></span>|<span data-ttu-id="535a1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="535a1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="535a1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="535a1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="535a1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="535a1-118">Request headers</span></span>
|<span data-ttu-id="535a1-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="535a1-119">Header</span></span>|<span data-ttu-id="535a1-120">Значение</span><span class="sxs-lookup"><span data-stu-id="535a1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="535a1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="535a1-121">Authorization</span></span>|<span data-ttu-id="535a1-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="535a1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="535a1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="535a1-123">Accept</span></span>|<span data-ttu-id="535a1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="535a1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="535a1-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="535a1-125">Request body</span></span>
<span data-ttu-id="535a1-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="535a1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="535a1-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="535a1-127">Response</span></span>
<span data-ttu-id="535a1-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="535a1-128">If successful, this method returns a `200 OK` response code and a collection of [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="535a1-129">Пример</span><span class="sxs-lookup"><span data-stu-id="535a1-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="535a1-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="535a1-130">Request</span></span>
<span data-ttu-id="535a1-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="535a1-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="535a1-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="535a1-132">Response</span></span>
<span data-ttu-id="535a1-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="535a1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1164

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsMobileMSI",
      "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
      "commandLine": "Command Line value",
      "productCode": "Product Code value",
      "productVersion": "Product Version value",
      "ignoreVersionDetection": true
    }
  ]
}
```



