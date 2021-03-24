---
title: Перечисление объектов iosVppApp
description: Список свойств и связей объектов iosVppApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 99d5d7462a5c4d64418693afdd6a033c9e483670
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144132"
---
# <a name="list-iosvppapps"></a><span data-ttu-id="90850-103">Перечисление объектов iosVppApp</span><span class="sxs-lookup"><span data-stu-id="90850-103">List iosVppApps</span></span>

<span data-ttu-id="90850-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90850-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90850-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90850-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90850-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90850-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90850-107">Список свойств и связей объектов [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="90850-107">List properties and relationships of the [iosVppApp](../resources/intune-apps-iosvppapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90850-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="90850-108">Prerequisites</span></span>
<span data-ttu-id="90850-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90850-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90850-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90850-111">Permission type</span></span>|<span data-ttu-id="90850-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90850-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90850-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90850-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90850-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90850-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="90850-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90850-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90850-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90850-116">Not supported.</span></span>|
|<span data-ttu-id="90850-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="90850-117">Application</span></span>|<span data-ttu-id="90850-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90850-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90850-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90850-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="90850-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="90850-120">Request headers</span></span>
|<span data-ttu-id="90850-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="90850-121">Header</span></span>|<span data-ttu-id="90850-122">Значение</span><span class="sxs-lookup"><span data-stu-id="90850-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90850-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="90850-123">Authorization</span></span>|<span data-ttu-id="90850-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90850-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90850-125">Accept</span><span class="sxs-lookup"><span data-stu-id="90850-125">Accept</span></span>|<span data-ttu-id="90850-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90850-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90850-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90850-127">Request body</span></span>
<span data-ttu-id="90850-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90850-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90850-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="90850-129">Response</span></span>
<span data-ttu-id="90850-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosVppApp](../resources/intune-apps-iosvppapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="90850-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppApp](../resources/intune-apps-iosvppapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90850-131">Пример</span><span class="sxs-lookup"><span data-stu-id="90850-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="90850-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="90850-132">Request</span></span>
<span data-ttu-id="90850-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90850-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="90850-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="90850-134">Response</span></span>
<span data-ttu-id="90850-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90850-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2509

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




