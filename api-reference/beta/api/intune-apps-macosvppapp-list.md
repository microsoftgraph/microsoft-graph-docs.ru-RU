---
title: Список Макосвппаппс
description: Список свойств и связей объектов Макосвппапп.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0a441f2a022fc6e759c2e7339a3e5e090692d02d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961982"
---
# <a name="list-macosvppapps"></a><span data-ttu-id="f91d9-103">Список Макосвппаппс</span><span class="sxs-lookup"><span data-stu-id="f91d9-103">List macOsVppApps</span></span>

> <span data-ttu-id="f91d9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f91d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f91d9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f91d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f91d9-106">Список свойств и связей объектов [макосвппапп](../resources/intune-apps-macosvppapp.md) .</span><span class="sxs-lookup"><span data-stu-id="f91d9-106">List properties and relationships of the [macOsVppApp](../resources/intune-apps-macosvppapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f91d9-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f91d9-107">Prerequisites</span></span>
<span data-ttu-id="f91d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f91d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f91d9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f91d9-110">Permission type</span></span>|<span data-ttu-id="f91d9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f91d9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f91d9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f91d9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f91d9-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f91d9-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f91d9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f91d9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f91d9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f91d9-115">Not supported.</span></span>|
|<span data-ttu-id="f91d9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f91d9-116">Application</span></span>|<span data-ttu-id="f91d9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f91d9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f91d9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f91d9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f91d9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f91d9-119">Request headers</span></span>
|<span data-ttu-id="f91d9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f91d9-120">Header</span></span>|<span data-ttu-id="f91d9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f91d9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f91d9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f91d9-122">Authorization</span></span>|<span data-ttu-id="f91d9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f91d9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f91d9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f91d9-124">Accept</span></span>|<span data-ttu-id="f91d9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f91d9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f91d9-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f91d9-126">Request body</span></span>
<span data-ttu-id="f91d9-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f91d9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f91d9-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="f91d9-128">Response</span></span>
<span data-ttu-id="f91d9-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [макосвппапп](../resources/intune-apps-macosvppapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f91d9-129">If successful, this method returns a `200 OK` response code and a collection of [macOsVppApp](../resources/intune-apps-macosvppapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f91d9-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f91d9-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f91d9-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f91d9-131">Request</span></span>
<span data-ttu-id="f91d9-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f91d9-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="f91d9-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f91d9-133">Response</span></span>
<span data-ttu-id="f91d9-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f91d9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2294

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





