---
title: Get androidStoreApp
description: Чтение свойств и связей объекта androidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e1158b9d56c7f4a095b2216c720a138e923d9728
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466662"
---
# <a name="get-androidstoreapp"></a><span data-ttu-id="85317-103">Get androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="85317-103">Get androidStoreApp</span></span>

<span data-ttu-id="85317-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85317-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85317-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85317-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85317-106">Чтение свойств и связей объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="85317-106">Read properties and relationships of the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85317-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="85317-107">Prerequisites</span></span>
<span data-ttu-id="85317-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85317-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85317-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85317-110">Permission type</span></span>|<span data-ttu-id="85317-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="85317-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85317-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85317-112">Delegated (work or school account)</span></span>|<span data-ttu-id="85317-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="85317-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="85317-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85317-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85317-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85317-115">Not supported.</span></span>|
|<span data-ttu-id="85317-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85317-116">Application</span></span>|<span data-ttu-id="85317-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85317-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85317-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85317-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="85317-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="85317-119">Optional query parameters</span></span>
<span data-ttu-id="85317-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="85317-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85317-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85317-121">Request headers</span></span>
|<span data-ttu-id="85317-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85317-122">Header</span></span>|<span data-ttu-id="85317-123">Значение</span><span class="sxs-lookup"><span data-stu-id="85317-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85317-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85317-124">Authorization</span></span>|<span data-ttu-id="85317-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85317-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85317-126">Accept</span><span class="sxs-lookup"><span data-stu-id="85317-126">Accept</span></span>|<span data-ttu-id="85317-127">application/json</span><span class="sxs-lookup"><span data-stu-id="85317-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85317-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="85317-128">Request body</span></span>
<span data-ttu-id="85317-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="85317-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85317-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="85317-130">Response</span></span>
<span data-ttu-id="85317-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="85317-131">If successful, this method returns a `200 OK` response code and [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85317-132">Пример</span><span class="sxs-lookup"><span data-stu-id="85317-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="85317-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="85317-133">Request</span></span>
<span data-ttu-id="85317-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85317-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="85317-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="85317-135">Response</span></span>
<span data-ttu-id="85317-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85317-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






