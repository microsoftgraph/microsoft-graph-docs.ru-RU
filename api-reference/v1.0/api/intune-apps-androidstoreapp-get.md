---
title: Get androidStoreApp
description: Чтение свойств и связей объекта androidStoreApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2339db20fe0359fc3949671c75a3330cf98488e0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833501"
---
# <a name="get-androidstoreapp"></a><span data-ttu-id="82adf-103">Get androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="82adf-103">Get androidStoreApp</span></span>

> <span data-ttu-id="82adf-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="82adf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="82adf-105">Чтение свойств и связей объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="82adf-105">Read properties and relationships of the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="82adf-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="82adf-106">Prerequisites</span></span>
<span data-ttu-id="82adf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82adf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82adf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82adf-109">Permission type</span></span>|<span data-ttu-id="82adf-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="82adf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82adf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82adf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="82adf-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="82adf-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="82adf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82adf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82adf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82adf-114">Not supported.</span></span>|
|<span data-ttu-id="82adf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82adf-115">Application</span></span>|<span data-ttu-id="82adf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82adf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82adf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82adf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="82adf-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="82adf-118">Optional query parameters</span></span>
<span data-ttu-id="82adf-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="82adf-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="82adf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82adf-120">Request headers</span></span>
|<span data-ttu-id="82adf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82adf-121">Header</span></span>|<span data-ttu-id="82adf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="82adf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82adf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="82adf-123">Authorization</span></span>|<span data-ttu-id="82adf-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="82adf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82adf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="82adf-125">Accept</span></span>|<span data-ttu-id="82adf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="82adf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82adf-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="82adf-127">Request body</span></span>
<span data-ttu-id="82adf-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="82adf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82adf-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="82adf-129">Response</span></span>
<span data-ttu-id="82adf-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="82adf-130">If successful, this method returns a `200 OK` response code and [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82adf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="82adf-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="82adf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="82adf-132">Request</span></span>
<span data-ttu-id="82adf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82adf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="82adf-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="82adf-134">Response</span></span>
<span data-ttu-id="82adf-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="82adf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1193

{
  "value": {
    "@odata.type": "#microsoft.graph.androidStoreApp",
    "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
    "packageId": "Package Id value",
    "appStoreUrl": "https://example.com/appStoreUrl/",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
      "v4_0": true,
      "v4_0_3": true,
      "v4_1": true,
      "v4_2": true,
      "v4_3": true,
      "v4_4": true,
      "v5_0": true,
      "v5_1": true
    }
  }
}
```



