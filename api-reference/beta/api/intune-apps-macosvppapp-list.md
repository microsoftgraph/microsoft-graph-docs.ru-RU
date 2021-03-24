---
title: Список macOsVppApps
description: Список свойств и связей объектов macOsVppApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0c7362b7e599b39c6575189aa8f16d8118ce8d71
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140373"
---
# <a name="list-macosvppapps"></a><span data-ttu-id="7d9eb-103">Список macOsVppApps</span><span class="sxs-lookup"><span data-stu-id="7d9eb-103">List macOsVppApps</span></span>

<span data-ttu-id="7d9eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d9eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7d9eb-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d9eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d9eb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7d9eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d9eb-107">Список свойств и связей объектов [macOsVppApp.](../resources/intune-apps-macosvppapp.md)</span><span class="sxs-lookup"><span data-stu-id="7d9eb-107">List properties and relationships of the [macOsVppApp](../resources/intune-apps-macosvppapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d9eb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7d9eb-108">Prerequisites</span></span>
<span data-ttu-id="7d9eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d9eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d9eb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d9eb-111">Permission type</span></span>|<span data-ttu-id="7d9eb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d9eb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d9eb-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d9eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d9eb-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d9eb-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7d9eb-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d9eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d9eb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d9eb-116">Not supported.</span></span>|
|<span data-ttu-id="7d9eb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7d9eb-117">Application</span></span>|<span data-ttu-id="7d9eb-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d9eb-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d9eb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d9eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="7d9eb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7d9eb-120">Request headers</span></span>
|<span data-ttu-id="7d9eb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7d9eb-121">Header</span></span>|<span data-ttu-id="7d9eb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7d9eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d9eb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d9eb-123">Authorization</span></span>|<span data-ttu-id="7d9eb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d9eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d9eb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7d9eb-125">Accept</span></span>|<span data-ttu-id="7d9eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7d9eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d9eb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d9eb-127">Request body</span></span>
<span data-ttu-id="7d9eb-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7d9eb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d9eb-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d9eb-129">Response</span></span>
<span data-ttu-id="7d9eb-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [macOsVppApp](../resources/intune-apps-macosvppapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7d9eb-130">If successful, this method returns a `200 OK` response code and a collection of [macOsVppApp](../resources/intune-apps-macosvppapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d9eb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7d9eb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d9eb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d9eb-132">Request</span></span>
<span data-ttu-id="7d9eb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d9eb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="7d9eb-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d9eb-134">Response</span></span>
<span data-ttu-id="7d9eb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d9eb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2359

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOsVppApp",
      "id": "10b95265-5265-10b9-6552-b9106552b910",
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
      "supersedingAppCount": 3,
      "supersededAppCount": 2,
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
      "vppTokenOrganizationName": "Vpp Token Organization Name value",
      "vppTokenAccountType": "education",
      "vppTokenAppleId": "Vpp Token Apple Id value",
      "bundleId": "Bundle Id value",
      "vppTokenId": "Vpp Token Id value",
      "revokeLicenseActionResults": [
        {
          "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
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




