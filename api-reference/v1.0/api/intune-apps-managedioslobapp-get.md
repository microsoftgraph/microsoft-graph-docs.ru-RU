---
title: Get managedIOSLobApp
description: Чтение свойств и связей объекта managedIOSLobApp.
ms.openlocfilehash: 1fce864ed1e627366e65a2d6e22d4fcb05713124
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025680"
---
# <a name="get-managedioslobapp"></a><span data-ttu-id="1188c-103">Get managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="1188c-103">Get managedIOSLobApp</span></span>

> <span data-ttu-id="1188c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1188c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1188c-105">Чтение свойств и связей объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="1188c-105">Read properties and relationships of the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1188c-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1188c-106">Prerequisites</span></span>
<span data-ttu-id="1188c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1188c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1188c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1188c-109">Permission type</span></span>|<span data-ttu-id="1188c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1188c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1188c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1188c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1188c-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1188c-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1188c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1188c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1188c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1188c-114">Not supported.</span></span>|
|<span data-ttu-id="1188c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1188c-115">Application</span></span>|<span data-ttu-id="1188c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1188c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1188c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1188c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1188c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1188c-118">Optional query parameters</span></span>
<span data-ttu-id="1188c-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1188c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1188c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1188c-120">Request headers</span></span>
|<span data-ttu-id="1188c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1188c-121">Header</span></span>|<span data-ttu-id="1188c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1188c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1188c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1188c-123">Authorization</span></span>|<span data-ttu-id="1188c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1188c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1188c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1188c-125">Accept</span></span>|<span data-ttu-id="1188c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1188c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1188c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1188c-127">Request body</span></span>
<span data-ttu-id="1188c-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1188c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1188c-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="1188c-129">Response</span></span>
<span data-ttu-id="1188c-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1188c-130">If successful, this method returns a `200 OK` response code and [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1188c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1188c-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1188c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1188c-132">Request</span></span>
<span data-ttu-id="1188c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1188c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="1188c-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="1188c-134">Response</span></span>
<span data-ttu-id="1188c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="1188c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1560

{
  "value": {
    "@odata.type": "#microsoft.graph.managedIOSLobApp",
    "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
    "appAvailability": "lineOfBusiness",
    "version": "Version value",
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
      "v12_0": true
    },
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "versionNumber": "Version Number value",
    "buildNumber": "Build Number value"
  }
}
```



