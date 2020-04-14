---
title: Get microsoftStoreForBusinessApp
description: Чтение свойств и связей объекта microsoftStoreForBusinessApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 24d5b4fb4f54f44db92f8831b7e7bf69e3f79cc4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43405138"
---
# <a name="get-microsoftstoreforbusinessapp"></a><span data-ttu-id="fc150-103">Get microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="fc150-103">Get microsoftStoreForBusinessApp</span></span>

<span data-ttu-id="fc150-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc150-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc150-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc150-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc150-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc150-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc150-107">Чтение свойств и связей объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="fc150-107">Read properties and relationships of the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc150-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fc150-108">Prerequisites</span></span>
<span data-ttu-id="fc150-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc150-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc150-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc150-111">Permission type</span></span>|<span data-ttu-id="fc150-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc150-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc150-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc150-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fc150-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc150-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fc150-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc150-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc150-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc150-116">Not supported.</span></span>|
|<span data-ttu-id="fc150-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="fc150-117">Application</span></span>|<span data-ttu-id="fc150-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc150-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc150-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc150-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fc150-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fc150-120">Optional query parameters</span></span>
<span data-ttu-id="fc150-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fc150-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fc150-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc150-122">Request headers</span></span>
|<span data-ttu-id="fc150-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fc150-123">Header</span></span>|<span data-ttu-id="fc150-124">Значение</span><span class="sxs-lookup"><span data-stu-id="fc150-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc150-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc150-125">Authorization</span></span>|<span data-ttu-id="fc150-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc150-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc150-127">Accept</span><span class="sxs-lookup"><span data-stu-id="fc150-127">Accept</span></span>|<span data-ttu-id="fc150-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fc150-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc150-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc150-129">Request body</span></span>
<span data-ttu-id="fc150-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fc150-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc150-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="fc150-131">Response</span></span>
<span data-ttu-id="fc150-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fc150-132">If successful, this method returns a `200 OK` response code and [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc150-133">Пример</span><span class="sxs-lookup"><span data-stu-id="fc150-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc150-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc150-134">Request</span></span>
<span data-ttu-id="fc150-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc150-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="fc150-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc150-136">Response</span></span>
<span data-ttu-id="fc150-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc150-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1397

{
  "value": {
    "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
    "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
    "productKey": "Product Key value",
    "licenseType": "online",
    "packageIdentityName": "Package Identity Name value",
    "licensingType": {
      "@odata.type": "microsoft.graph.vppLicensingType",
      "supportUserLicensing": true,
      "supportDeviceLicensing": true,
      "supportsUserLicensing": true,
      "supportsDeviceLicensing": true
    }
  }
}
```



