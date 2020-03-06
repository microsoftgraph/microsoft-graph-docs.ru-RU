---
title: Перечисление объектов iosVppApp
description: Список свойств и связей объектов iosVppApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7a57fa3811b6276afd03dc5de080a4409ef646ec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516499"
---
# <a name="list-iosvppapps"></a><span data-ttu-id="16365-103">Перечисление объектов iosVppApp</span><span class="sxs-lookup"><span data-stu-id="16365-103">List iosVppApps</span></span>

<span data-ttu-id="16365-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16365-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16365-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="16365-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16365-106">Список свойств и связей объектов [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="16365-106">List properties and relationships of the [iosVppApp](../resources/intune-apps-iosvppapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16365-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="16365-107">Prerequisites</span></span>
<span data-ttu-id="16365-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16365-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16365-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16365-110">Permission type</span></span>|<span data-ttu-id="16365-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="16365-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16365-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16365-112">Delegated (work or school account)</span></span>|<span data-ttu-id="16365-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="16365-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="16365-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16365-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16365-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16365-115">Not supported.</span></span>|
|<span data-ttu-id="16365-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16365-116">Application</span></span>|<span data-ttu-id="16365-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16365-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16365-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16365-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="16365-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="16365-119">Request headers</span></span>
|<span data-ttu-id="16365-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16365-120">Header</span></span>|<span data-ttu-id="16365-121">Значение</span><span class="sxs-lookup"><span data-stu-id="16365-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16365-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="16365-122">Authorization</span></span>|<span data-ttu-id="16365-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16365-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16365-124">Accept</span><span class="sxs-lookup"><span data-stu-id="16365-124">Accept</span></span>|<span data-ttu-id="16365-125">application/json</span><span class="sxs-lookup"><span data-stu-id="16365-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16365-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16365-126">Request body</span></span>
<span data-ttu-id="16365-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="16365-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16365-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="16365-128">Response</span></span>
<span data-ttu-id="16365-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosVppApp](../resources/intune-apps-iosvppapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="16365-129">If successful, this method returns a `200 OK` response code and a collection of [iosVppApp](../resources/intune-apps-iosvppapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16365-130">Пример</span><span class="sxs-lookup"><span data-stu-id="16365-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="16365-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="16365-131">Request</span></span>
<span data-ttu-id="16365-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16365-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="16365-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="16365-133">Response</span></span>
<span data-ttu-id="16365-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16365-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




