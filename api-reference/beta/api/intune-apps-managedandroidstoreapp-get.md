---
title: Get managedAndroidStoreApp
description: Чтение свойств и связей объекта managedAndroidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0c7b48c551a985c6198ad22a60fcef5b8d41897d
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157290"
---
# <a name="get-managedandroidstoreapp"></a><span data-ttu-id="d2ba2-103">Get managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="d2ba2-103">Get managedAndroidStoreApp</span></span>

<span data-ttu-id="d2ba2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2ba2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2ba2-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2ba2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2ba2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2ba2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2ba2-107">Чтение свойств и связей объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="d2ba2-107">Read properties and relationships of the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2ba2-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d2ba2-108">Prerequisites</span></span>
<span data-ttu-id="d2ba2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2ba2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2ba2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2ba2-111">Permission type</span></span>|<span data-ttu-id="d2ba2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2ba2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2ba2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2ba2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d2ba2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2ba2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d2ba2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2ba2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2ba2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2ba2-116">Not supported.</span></span>|
|<span data-ttu-id="d2ba2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2ba2-117">Application</span></span>|<span data-ttu-id="d2ba2-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2ba2-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2ba2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2ba2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d2ba2-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d2ba2-120">Optional query parameters</span></span>
<span data-ttu-id="d2ba2-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d2ba2-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2ba2-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2ba2-122">Request headers</span></span>
|<span data-ttu-id="d2ba2-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2ba2-123">Header</span></span>|<span data-ttu-id="d2ba2-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d2ba2-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2ba2-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2ba2-125">Authorization</span></span>|<span data-ttu-id="d2ba2-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2ba2-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2ba2-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d2ba2-127">Accept</span></span>|<span data-ttu-id="d2ba2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d2ba2-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2ba2-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2ba2-129">Request body</span></span>
<span data-ttu-id="d2ba2-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2ba2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2ba2-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2ba2-131">Response</span></span>
<span data-ttu-id="d2ba2-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d2ba2-132">If successful, this method returns a `200 OK` response code and [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2ba2-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d2ba2-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2ba2-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2ba2-134">Request</span></span>
<span data-ttu-id="d2ba2-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2ba2-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="d2ba2-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2ba2-136">Response</span></span>
<span data-ttu-id="d2ba2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2ba2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1652

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
    "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
    "appAvailability": "lineOfBusiness",
    "version": "Version value",
    "packageId": "Package Id value",
    "appStoreUrl": "https://example.com/appStoreUrl/",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
      "v4_0": true,
      "v4_0_3": true,
      "v4_1": true,
      "v4_2": true,
      "v4_3": true,
      "v4_4": true,
      "v5_0": true,
      "v5_1": true,
      "v6_0": true,
      "v7_0": true,
      "v7_1": true,
      "v8_0": true,
      "v8_1": true,
      "v9_0": true,
      "v10_0": true,
      "v11_0": true
    }
  }
}
```




