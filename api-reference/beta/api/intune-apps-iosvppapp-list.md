---
title: Перечисление объектов iosVppApp
description: Список свойств и связей объектов iosVppApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0d1a3a8bd24440a57f83948107bde037453b4960
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33936898"
---
# <a name="list-iosvppapps"></a><span data-ttu-id="0d257-103">Перечисление объектов iosVppApp</span><span class="sxs-lookup"><span data-stu-id="0d257-103">List iosVppApps</span></span>

> <span data-ttu-id="0d257-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d257-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d257-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d257-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d257-106">Список свойств и связей объектов [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d257-106">List properties and relationships of the [iosVppApp](../resources/intune-apps-iosvppapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d257-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0d257-107">Prerequisites</span></span>
<span data-ttu-id="0d257-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d257-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d257-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d257-110">Permission type</span></span>|<span data-ttu-id="0d257-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d257-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d257-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d257-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0d257-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d257-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0d257-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d257-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d257-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d257-115">Not supported.</span></span>|
|<span data-ttu-id="0d257-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d257-116">Application</span></span>|<span data-ttu-id="0d257-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d257-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d257-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d257-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0d257-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d257-119">Request headers</span></span>
|<span data-ttu-id="0d257-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d257-120">Header</span></span>|<span data-ttu-id="0d257-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0d257-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d257-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d257-122">Authorization</span></span>|<span data-ttu-id="0d257-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d257-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d257-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0d257-124">Accept</span></span>|<span data-ttu-id="0d257-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0d257-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d257-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0d257-126">Request body</span></span>
<span data-ttu-id="0d257-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0d257-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d257-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d257-128">Response</span></span>
<span data-ttu-id="0d257-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosVppApp](../resources/intune-apps-iosvppapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0d257-129">If successful, this method returns a `200 OK` response code and a collection of [iosVppApp](../resources/intune-apps-iosvppapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d257-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0d257-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d257-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d257-131">Request</span></span>
<span data-ttu-id="0d257-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d257-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="0d257-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d257-133">Response</span></span>
<span data-ttu-id="0d257-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d257-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2444

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
      "uploadState": 11,
      "publishingState": "processing",
      "isAssigned": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "dependentAppCount": 1,
      "usedLicenseCount": 0,
      "totalLicenseCount": 1,
      "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "licensingType": {
        "@odata.type": "microsoft.graph.vppLicensingType",
        "supportUserLicensing": true,
        "supportDeviceLicensing": true,
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
      "bundleId": "Bundle Id value",
      "vppTokenId": "Vpp Token Id value",
      "revokeLicenseActionResults": [
        {
          "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
          "userId": "User Id value",
          "managedDeviceId": "Managed Device Id value",
          "totalLicensesCount": 2,
          "failedLicensesCount": 3,
          "actionFailureReason": "appleFailure",
          "actionName": "Action Name value",
          "actionState": "pending",
          "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
          "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
        }
      ]
    }
  ]
}
```




