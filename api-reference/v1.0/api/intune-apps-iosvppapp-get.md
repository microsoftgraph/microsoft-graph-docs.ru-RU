---
title: Get iosVppApp
description: Чтение свойств и связей объекта iosVppApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: be8117c72c3edb8410c4e5f2f9e6287469c3d33c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960723"
---
# <a name="get-iosvppapp"></a><span data-ttu-id="8bb76-103">Get iosVppApp</span><span class="sxs-lookup"><span data-stu-id="8bb76-103">Get iosVppApp</span></span>

> <span data-ttu-id="8bb76-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8bb76-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8bb76-105">Чтение свойств и связей объекта [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="8bb76-105">Read properties and relationships of the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8bb76-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8bb76-106">Prerequisites</span></span>
<span data-ttu-id="8bb76-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bb76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bb76-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8bb76-109">Permission type</span></span>|<span data-ttu-id="8bb76-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8bb76-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bb76-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8bb76-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8bb76-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb76-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8bb76-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8bb76-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bb76-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bb76-114">Not supported.</span></span>|
|<span data-ttu-id="8bb76-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8bb76-115">Application</span></span>|<span data-ttu-id="8bb76-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bb76-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bb76-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8bb76-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8bb76-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8bb76-118">Optional query parameters</span></span>
<span data-ttu-id="8bb76-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8bb76-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8bb76-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8bb76-120">Request headers</span></span>
|<span data-ttu-id="8bb76-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8bb76-121">Header</span></span>|<span data-ttu-id="8bb76-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8bb76-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bb76-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bb76-123">Authorization</span></span>|<span data-ttu-id="8bb76-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8bb76-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bb76-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8bb76-125">Accept</span></span>|<span data-ttu-id="8bb76-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8bb76-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bb76-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8bb76-127">Request body</span></span>
<span data-ttu-id="8bb76-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8bb76-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8bb76-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="8bb76-129">Response</span></span>
<span data-ttu-id="8bb76-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosVppApp](../resources/intune-apps-iosvppapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8bb76-130">If successful, this method returns a `200 OK` response code and [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bb76-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8bb76-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8bb76-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bb76-132">Request</span></span>
<span data-ttu-id="8bb76-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8bb76-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="8bb76-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bb76-134">Response</span></span>
<span data-ttu-id="8bb76-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8bb76-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1487

{
  "value": {
    "@odata.type": "#microsoft.graph.iosVppApp",
    "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
    "usedLicenseCount": 0,
    "totalLicenseCount": 1,
    "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
    "appStoreUrl": "https://example.com/appStoreUrl/",
    "licensingType": {
      "@odata.type": "microsoft.graph.vppLicensingType",
      "supportsUserLicensing": true,
      "supportsDeviceLicensing": true
    },
    "applicableDeviceType": {
      "@odata.type": "microsoft.graph.iosDeviceType",
      "iPad": true,
      "iPhoneAndIPod": true
    },
    "vppTokenOrganizationName": "Vpp Token Organization Name value",
    "vppTokenAccountType": "education",
    "vppTokenAppleId": "Vpp Token Apple Id value",
    "bundleId": "Bundle Id value"
  }
}
```



