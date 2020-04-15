---
title: Перечисление объектов windowsMobileMSI
description: Список свойств и связей объектов windowsMobileMSI.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 28bf3e4c513b5818ab2461fd23a453355f0405e3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43464511"
---
# <a name="list-windowsmobilemsis"></a><span data-ttu-id="2b695-103">Перечисление объектов windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="2b695-103">List windowsMobileMSIs</span></span>

<span data-ttu-id="2b695-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b695-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b695-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b695-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b695-106">Список свойств и связей объектов [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="2b695-106">List properties and relationships of the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b695-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2b695-107">Prerequisites</span></span>
<span data-ttu-id="2b695-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b695-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b695-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b695-110">Permission type</span></span>|<span data-ttu-id="2b695-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b695-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b695-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b695-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2b695-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b695-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2b695-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b695-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b695-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b695-115">Not supported.</span></span>|
|<span data-ttu-id="2b695-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b695-116">Application</span></span>|<span data-ttu-id="2b695-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b695-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b695-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b695-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="2b695-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2b695-119">Request headers</span></span>
|<span data-ttu-id="2b695-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b695-120">Header</span></span>|<span data-ttu-id="2b695-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2b695-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b695-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b695-122">Authorization</span></span>|<span data-ttu-id="2b695-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b695-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b695-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2b695-124">Accept</span></span>|<span data-ttu-id="2b695-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2b695-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b695-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2b695-126">Request body</span></span>
<span data-ttu-id="2b695-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b695-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b695-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b695-128">Response</span></span>
<span data-ttu-id="2b695-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2b695-129">If successful, this method returns a `200 OK` response code and a collection of [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b695-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2b695-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b695-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b695-131">Request</span></span>
<span data-ttu-id="2b695-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b695-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="2b695-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b695-133">Response</span></span>
<span data-ttu-id="2b695-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b695-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






