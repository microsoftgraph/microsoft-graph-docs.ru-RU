---
title: Перечисление объектов iosVppApp
description: Список свойств и связей объектов iosVppApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7742a542f97a9135cb15c7744badcd1284c62c98
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843150"
---
# <a name="list-iosvppapps"></a><span data-ttu-id="2f26b-103">Перечисление объектов iosVppApp</span><span class="sxs-lookup"><span data-stu-id="2f26b-103">List iosVppApps</span></span>

> <span data-ttu-id="2f26b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2f26b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f26b-105">Список свойств и связей объектов [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f26b-105">List properties and relationships of the [iosVppApp](../resources/intune-apps-iosvppapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2f26b-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2f26b-106">Prerequisites</span></span>
<span data-ttu-id="2f26b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f26b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f26b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f26b-109">Permission type</span></span>|<span data-ttu-id="2f26b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f26b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f26b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f26b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2f26b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f26b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2f26b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f26b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f26b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f26b-114">Not supported.</span></span>|
|<span data-ttu-id="2f26b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f26b-115">Application</span></span>|<span data-ttu-id="2f26b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f26b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f26b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f26b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="2f26b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f26b-118">Request headers</span></span>
|<span data-ttu-id="2f26b-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f26b-119">Header</span></span>|<span data-ttu-id="2f26b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2f26b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f26b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f26b-121">Authorization</span></span>|<span data-ttu-id="2f26b-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2f26b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f26b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2f26b-123">Accept</span></span>|<span data-ttu-id="2f26b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2f26b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f26b-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2f26b-125">Request body</span></span>
<span data-ttu-id="2f26b-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2f26b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f26b-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f26b-127">Response</span></span>
<span data-ttu-id="2f26b-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosVppApp](../resources/intune-apps-iosvppapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2f26b-128">If successful, this method returns a `200 OK` response code and a collection of [iosVppApp](../resources/intune-apps-iosvppapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f26b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="2f26b-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="2f26b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f26b-130">Request</span></span>
<span data-ttu-id="2f26b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f26b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="2f26b-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="2f26b-132">Response</span></span>
<span data-ttu-id="2f26b-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2f26b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1575

{
  "value": [
    {
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
  ]
}
```



