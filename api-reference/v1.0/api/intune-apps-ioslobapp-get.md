---
title: Get iosLobApp
description: Чтение свойств и связей объекта iosLobApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4e592a42dda632a55e89b4f711ba6a77913e7302
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355626"
---
# <a name="get-ioslobapp"></a><span data-ttu-id="96f78-103">Get iosLobApp</span><span class="sxs-lookup"><span data-stu-id="96f78-103">Get iosLobApp</span></span>

> <span data-ttu-id="96f78-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="96f78-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96f78-105">Чтение свойств и связей объекта [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="96f78-105">Read properties and relationships of the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96f78-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="96f78-106">Prerequisites</span></span>
<span data-ttu-id="96f78-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="96f78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="96f78-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96f78-109">Permission type</span></span>|<span data-ttu-id="96f78-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="96f78-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96f78-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96f78-111">Delegated (work or school account)</span></span>|<span data-ttu-id="96f78-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="96f78-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="96f78-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96f78-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96f78-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96f78-114">Not supported.</span></span>|
|<span data-ttu-id="96f78-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96f78-115">Application</span></span>|<span data-ttu-id="96f78-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="96f78-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96f78-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96f78-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="96f78-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="96f78-118">Optional query parameters</span></span>
<span data-ttu-id="96f78-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="96f78-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96f78-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96f78-120">Request headers</span></span>
|<span data-ttu-id="96f78-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="96f78-121">Header</span></span>|<span data-ttu-id="96f78-122">Значение</span><span class="sxs-lookup"><span data-stu-id="96f78-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96f78-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96f78-123">Authorization</span></span>|<span data-ttu-id="96f78-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96f78-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96f78-125">Accept</span><span class="sxs-lookup"><span data-stu-id="96f78-125">Accept</span></span>|<span data-ttu-id="96f78-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96f78-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96f78-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96f78-127">Request body</span></span>
<span data-ttu-id="96f78-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="96f78-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96f78-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="96f78-129">Response</span></span>
<span data-ttu-id="96f78-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosLobApp](../resources/intune-apps-ioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="96f78-130">If successful, this method returns a `200 OK` response code and [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96f78-131">Пример</span><span class="sxs-lookup"><span data-stu-id="96f78-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="96f78-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="96f78-132">Request</span></span>
<span data-ttu-id="96f78-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96f78-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="96f78-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="96f78-134">Response</span></span>
<span data-ttu-id="96f78-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="96f78-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1500

{
  "value": {
    "@odata.type": "#microsoft.graph.iosLobApp",
    "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
    "bundleId": "Bundle Id value",
    "applicableDeviceType": {
      "@odata.type": "microsoft.graph.iosDeviceType",
      "iPad": true,
      "iPhoneAndIPod": true
    },
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
      "v8_0": true,
      "v9_0": true,
      "v10_0": true,
      "v11_0": true,
      "v12_0": true,
      "v13_0": true
    },
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "versionNumber": "Version Number value",
    "buildNumber": "Build Number value"
  }
}
```




