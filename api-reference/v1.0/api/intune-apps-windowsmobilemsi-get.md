---
title: Get windowsMobileMSI
description: Чтение свойств и связей объекта windowsMobileMSI.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dbe9088261e76cd687ed6ae2dd7cd576f0b63173
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975331"
---
# <a name="get-windowsmobilemsi"></a><span data-ttu-id="ad704-103">Get windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="ad704-103">Get windowsMobileMSI</span></span>

> <span data-ttu-id="ad704-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ad704-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad704-105">Чтение свойств и связей объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="ad704-105">Read properties and relationships of the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad704-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ad704-106">Prerequisites</span></span>
<span data-ttu-id="ad704-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad704-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad704-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad704-109">Permission type</span></span>|<span data-ttu-id="ad704-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad704-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad704-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad704-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ad704-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad704-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ad704-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad704-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad704-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad704-114">Not supported.</span></span>|
|<span data-ttu-id="ad704-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad704-115">Application</span></span>|<span data-ttu-id="ad704-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad704-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad704-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad704-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ad704-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ad704-118">Optional query parameters</span></span>
<span data-ttu-id="ad704-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ad704-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ad704-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad704-120">Request headers</span></span>
|<span data-ttu-id="ad704-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ad704-121">Header</span></span>|<span data-ttu-id="ad704-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ad704-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad704-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad704-123">Authorization</span></span>|<span data-ttu-id="ad704-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad704-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad704-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ad704-125">Accept</span></span>|<span data-ttu-id="ad704-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ad704-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad704-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad704-127">Request body</span></span>
<span data-ttu-id="ad704-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ad704-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad704-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad704-129">Response</span></span>
<span data-ttu-id="ad704-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ad704-130">If successful, this method returns a `200 OK` response code and [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad704-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ad704-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad704-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad704-132">Request</span></span>
<span data-ttu-id="ad704-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad704-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="ad704-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad704-134">Response</span></span>
<span data-ttu-id="ad704-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad704-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1098

{
  "value": {
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
}
```



