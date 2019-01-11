---
title: Get microsoftStoreForBusinessApp
description: Чтение свойств и связей объекта microsoftStoreForBusinessApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 50975e2a3abc73ad61f457f155c2bc4ae3f484f8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859614"
---
# <a name="get-microsoftstoreforbusinessapp"></a><span data-ttu-id="a8248-103">Get microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="a8248-103">Get microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="a8248-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a8248-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8248-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8248-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8248-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a8248-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8248-107">Чтение свойств и связей объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="a8248-107">Read properties and relationships of the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a8248-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a8248-108">Prerequisites</span></span>
<span data-ttu-id="a8248-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8248-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8248-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8248-111">Permission type</span></span>|<span data-ttu-id="a8248-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8248-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8248-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8248-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8248-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8248-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a8248-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8248-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8248-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8248-116">Not supported.</span></span>|
|<span data-ttu-id="a8248-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8248-117">Application</span></span>|<span data-ttu-id="a8248-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8248-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8248-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8248-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a8248-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a8248-120">Optional query parameters</span></span>
<span data-ttu-id="a8248-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a8248-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a8248-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8248-122">Request headers</span></span>
|<span data-ttu-id="a8248-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a8248-123">Header</span></span>|<span data-ttu-id="a8248-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a8248-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8248-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8248-125">Authorization</span></span>|<span data-ttu-id="a8248-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a8248-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8248-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a8248-127">Accept</span></span>|<span data-ttu-id="a8248-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a8248-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8248-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a8248-129">Request body</span></span>
<span data-ttu-id="a8248-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a8248-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8248-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8248-131">Response</span></span>
<span data-ttu-id="a8248-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a8248-132">If successful, this method returns a `200 OK` response code and [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8248-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a8248-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="a8248-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8248-134">Request</span></span>
<span data-ttu-id="a8248-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8248-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="a8248-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8248-136">Response</span></span>
<span data-ttu-id="a8248-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a8248-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1032

{
  "value": {
    "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
    "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
    "usedLicenseCount": 0,
    "totalLicenseCount": 1,
    "productKey": "Product Key value",
    "licenseType": "online",
    "packageIdentityName": "Package Identity Name value"
  }
}
```





