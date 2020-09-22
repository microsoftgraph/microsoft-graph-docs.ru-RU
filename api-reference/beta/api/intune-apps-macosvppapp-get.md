---
title: Получение Макосвппапп
description: Чтение свойств и связей объекта Макосвппапп.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2813619c21a0b51db3e6336eb6d9db9ed005fdf7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48011951"
---
# <a name="get-macosvppapp"></a><span data-ttu-id="ce213-103">Получение Макосвппапп</span><span class="sxs-lookup"><span data-stu-id="ce213-103">Get macOsVppApp</span></span>

<span data-ttu-id="ce213-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce213-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce213-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce213-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce213-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ce213-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce213-107">Чтение свойств и связей объекта [макосвппапп](../resources/intune-apps-macosvppapp.md) .</span><span class="sxs-lookup"><span data-stu-id="ce213-107">Read properties and relationships of the [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce213-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ce213-108">Prerequisites</span></span>
<span data-ttu-id="ce213-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce213-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce213-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce213-111">Permission type</span></span>|<span data-ttu-id="ce213-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce213-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce213-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce213-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ce213-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce213-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ce213-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce213-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce213-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce213-116">Not supported.</span></span>|
|<span data-ttu-id="ce213-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce213-117">Application</span></span>|<span data-ttu-id="ce213-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce213-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce213-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce213-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ce213-120">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="ce213-120">Optional query parameters</span></span>
<span data-ttu-id="ce213-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ce213-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce213-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce213-122">Request headers</span></span>
|<span data-ttu-id="ce213-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ce213-123">Header</span></span>|<span data-ttu-id="ce213-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ce213-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce213-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce213-125">Authorization</span></span>|<span data-ttu-id="ce213-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce213-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce213-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ce213-127">Accept</span></span>|<span data-ttu-id="ce213-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ce213-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce213-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ce213-129">Request body</span></span>
<span data-ttu-id="ce213-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ce213-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce213-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce213-131">Response</span></span>
<span data-ttu-id="ce213-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [макосвппапп](../resources/intune-apps-macosvppapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ce213-132">If successful, this method returns a `200 OK` response code and [macOsVppApp](../resources/intune-apps-macosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce213-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ce213-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce213-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce213-134">Request</span></span>
<span data-ttu-id="ce213-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce213-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="ce213-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce213-136">Response</span></span>
<span data-ttu-id="ce213-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ce213-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2231

{
  "value": {
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
}
```






